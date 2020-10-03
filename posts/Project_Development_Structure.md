You've got a bunch of Software Developers and you've got an idea, so how do you make that idea a reality? What are the steps involved?

A lot of naive developers just dive right in, pick their favourite language and start writing code.

Don't be like these people.

Be smart, be sensible. Here's the steps:

1. Gathering Requirements
2. Requirements Analysis
3. Modelling
4. Architecture & Design
5. Technology Decisions
6. Platform & Networking
7. Proof of Concept
8. Subsequent Project Planning
9. Development
10. Adoption

## Gathering Requirements

Pretty much a given, but the first thing you need to do with your idea, is gather the requirements for what your thing needs to do. It doesn't have to be in formal [User Stories](https://en.wikipedia.org/wiki/User_story) yet, but writing a big document detailing your vision for your idea is a good start.

If you have prospective users, then talk to them and find out what problems they have or features they would want to see from your idea. Make questionnaires, conduct interviews, engage and observe your users doing whatever activity they would normally do that your idea would aim to solve.

Ultimately, you're trying to figure out how to best solve the problem that your idea is aiming to solve. That way, you get to know how to move forward with your idea, and in what form your idea will need to be realised - which might not be a piece of software! It's important to be open to the concept that your idea is a bad idea.  
By the way, if you're not trying to solve a problem, consider NOT making your idea a reality, as it's unlikely to be used and will likely just add to the bureacratic mess of systems and solutions that already exist in modern society today.

## Requirements Analysis

Once you have your idea laid out and fully described, you're going to want first figure out whether it's already been done before. What solutions already exist on the marketplace? Do they fully encompass your vision? What differentiates your idea from theirs? If they are already established and yours is different and starts to succeed, what's preventing your competition from just implementing your differentiating features and taking your users?  
Basically: _**Figure out your "gap in the market" and then figure out whether you're going to be able to hold onto that gap**_ because it takes a lot of time, effort and money to make ideas real and if you're idea is doomed from the beginning then it's better to save that time, effort and money for something more worthwhile.

If you're going ahead with your idea, figure out the answers to the following questions:

- Who are your users?
- How do your users interact with your thing? Do you need a UI? If so, what form is that UI taking? An mobile app? A website? Hands-free device like an Alexa or Google Home?
- How do your users adopt using your thing? Software installation? Subscription service? Buying it from a shop? Signing up for a user account?
- Are there any business-related limitations? Skillset amongst developers? Budget? Technical? Legal? Security?

Lastly, formalise your requirements. Usually, this means putting your requirements into [User Stories](https://en.wikipedia.org/wiki/User_story), in the form of:

As a `THING/PERSON`, I want to `ACTION`, because `REASON`.

Finally, prioritise your Requirements/User Stories. MoSCoW analysis helps here, but generally you should have an idea of what you're going to need to build first and what can be left for later.

## Modelling

A continuation of Requirements Analysis, of sorts. Modelling involves figuring out what are the core objects, functions, files (, etc.) of your idea. For most systems, this comes in the form of "Objects" and you will create an "Object Model" which will act as the foundation on which your end product will be designed around. However, not all products are Object-Oriented and so you should think carefully about what model your system needs and what form that should take. 

This will ultimately affect technology and programming language choices.

## Architecture & Design

Once you've figured out what you're application is going to be doing and the foundation that your solution is based on, you need to architect/design your solution.  
Generally this comes in two tiers:

- Solution-level
- System-level

where a _Solution_ is made up of multiple _Systems_. For example, [Twitter](https://twitter.com/) is a _Solution_ and the APIs, Mobile Apps, Websites, Databases, etc. are the _Systems_ that make up that the Twitter _Solution_.

_**At this stage, we only want to design the Solution-level Architecture.**_  
This involves figuring out how to solve your problem, but at an abstract level.  
For example, if you wanted to build a Notes solution, like Google Keep or Apple's Notes, you're abstract design might look something like:

- Mobile App
- Web UI
- API for [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) operations
- Database for storing notes
- Smart home integration/application for Hands-free note-taking

Notice how we haven't made any technology decisions? That's the point of Solution-level architecture: How you split up your Solution into the various Systems for how you're going to solve your overall problem.  
Each System should have a list of basic requirements placed on it by this design for how each System will be accessible by any other System. These should not be technology-related but instead simple, abstract design decisions such as: _"The API should be REST API that will take HTTP requests from any client-platform (web, mobile, etc.)."_  
This sort of proactive decision-making leads to a cleaner, more elegantly-coupled Solution and the removal of the need of any "Integration solution" (_shudder_).

If you have a UI, you'll want to decide how your UI is going to look at this point, too. This will affect the technologies that your UI developers will use to develop to that design.  
2 of the most important things to think about when designing a UI are User Experience (UX) and Accessibility (A11y). It's very nice to have a pretty looking UI but if people hate using it or physically CAN'T use it, then your UI is useless.

## Technology Decisions

Technology decisions are made at the System-level, and dictate the System-level Architecture.

Combining the requirements given to a System from the Solution-level Architectural Design, the original Solution requirements, any Modelling already done, and the limitations put on the Team who will be managing the System in question, the Team should have enough information to architect how they want to implement the System.

For example: For team of Java developers building a simple REST API that interacts with a Database, the team might decide to use [Spring](https://spring.io/), using [Spring Data REST](https://spring.io/projects/spring-data-rest), and then they'll roll their own ORM/Database integration (not something I'd usually recommend, but hey, it's an example).  
This will likely result in a layered application where you have a bunch of REST Controllers to take in HTTP Requests, some internal services that provide data to the Controllers, and the Database/ORM layer that provides the interface between the services and the Database.

## Platform & Networking

To actually run your Systems, you need platforms for those Systems to be deployed to, and you need to network these Systems together.

For platforms:

- Mobile apps are deployed to Mobile Operating Systems
- Websites are deployed to Servers of some kind (e.g. Serverless Functions, Containers, VMs, or physical Servers)
- APIs are also deployed to Servers of some kind.
- Databases are either managed services (i.e. on a Cloud Provider's platform) or deployed to servers of some kind.
- Smart-home integrations are deployed as Skills/Actions via the Smart-home device provider's console.

Even if you're using a completely managed solution, like Serverless or Android, there are still elements of compiling, packaging and configuration involved in engineering for that platform. It is best practice nowadays to drive all of this Platform Engineering through code, even for your Server Infrastructure (see: [Infrastructure as Code](https://en.wikipedia.org/wiki/Infrastructure_as_code)).

Figuring out how you're going to be building, deploying, maintaining and configuring your platform and your applications for your platform is incredibily important and affects how scalable, resilient and cost-effective your Solution will be.

Then you'll have to figure out how to Network your platforms together. Usually this is in the form of HTTPS requests over the Internet and within VPCs, but if you're going to be integrating with 3rd party platforms or on-premise infrastructure, you'll need to think about how you're going to securely integrate with these platforms so that they don't become networking bottle-necks or vulnerabilities that make your Solution slow and/or at risk of malicious exploitation.

## Proof of Concept

Now that you're done designing, it's time to build something.  
Start small and build just a few of the most important features of your Solution.

This will give you an idea for how good your technology decisions were and help you make any decisions about what sort of changes you'd like to make based on your first-hand experience of building your Proof of Concept.

It's expected that this PoC Solution will be buggy and ugly, but you should feel confident that ALL of those bugs and ugliness will be fixed in the development of your Solution. If you're worried about something now, then you'll want to discuss changing/improving it.

## Subsequent Project Planning

After having a taste of development and making a bunch mistakes in getting started, _now_ is the time to make those changes and improvements to your Architecture, Design and Systems to ensure that they are going to achieve the final goal of satisfying your user's desires.

Speaking of which, if you are making changes, then talk to your users about those changes and how they will affect the final product. Get their input as to whether they like, are indifferent or don't like the changes you're proposing. From this feedback, you should be able to architect and design solutions to your Proof of Concept problems that either adhere to the desires from the Users or at the very least provide a compromise.

## Development

Go build the fucking thing.

A Team should decide how they want to work together, but generally Agile teams using a somewhat flexible implementation of the SCRUM methodology (i.e. Sprints, Retros, etc.) has become industry-standard (2019).

It's a good to idea to build the Systems incrementally and respond to the changes of requirements and demands/dependencies from other Systems, hence why SCRUM is often implemented to break up this work into Sprints of 2+ weeks.

## Adoption

Once you've built the Solution, or at least the [Minimum Viable Product](https://en.wikipedia.org/wiki/Minimum_viable_product) of the Solution, you'll want to start rolling it out for User's to start using it.

Like with everything, start small and build up.  
This could come in multiple forms such as:

- Putting your Solution into Beta for your Users to test out.
- Only allowing a subset (5-20%) of your prospective Users to install your product and use it.

After proving your Solution works in a Production environemnt, and developing fixes & improvements to ensure resilience, scalability and usability: Roll your Solution out to all your Users and continue development to ensure your Solution retains is security, performance, 

If you're building a public product, Adoption for you means deploying your Solution to a scalable Production environment and then start running your marketing campaigns to get User's on-board.

---

If you're interested in how to Manage and Empower Software Engineering Teams when building Solutions, please check [this blog](/post/1574814665000).

---

Happy developing!

~ Harm x