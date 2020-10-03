## Cutting to the chase

Here's the basic component upgrade:

| Component                    | Old                                | New                                                                        |
| ---------------------------- | ---------------------------------- | -------------------------------------------------------------------------- |
| CPU                          | Intel i5-3570K                     | AMD Ryzen 5 3600X                                                          |
| RAM                          | 16GB Corsair Vengeance DDR3        | 16GB Corsair Vengeance LPX DDR4                                            |
| Motherboard                  | ASUS P8-Z77-V LX                   | ASUS ROG Strix B450-F Gaming                                               |
| GPU                          | EVGA Nvidia GeForce GTX 780 Ti     | Sapphire Radeon RX 5700                                                    |
| Sound Card / Audio Interface | M-Audio Delta 66 (w/ Omnibox)      | None                                                                       |
| PSU                          | Corsair RM850x                     | ---                                                                        |
| Storage                      | 1x 1TB HDD, 1x 2TB HDD, 1x 3TB HDD | 1x 240GB SSD, 1x 2TB HDD, 1x 3TB HDD                                       |
| CPU Cooling                  | Corsair H80                        | AMD Wraith Spire (Stock)                                                   |
| Tower Cooling                | 2x 120mm Fans                      | 3x 140mm Fans                                                              |
| Optical Drives               | LG 24x DVD Rewriter                | LG 14X Blu-ray M-Disc, LG 24x DVD Rewriter, STW 5.25" Internal Card Reader |
| Case                         | Bitfenix Merc Beta Midi            | Fractal Design Define XL R2                                                |
| Monitors                     | 1x BenQ GL2450, 1x BenQ GL2250     | 1x BenQ GL2450                                                             |
| Mouse                        | Maplin - Wireless                  | CSL SM-800                                                                 |
| Keyboard                     | Maplin - Wireless                  | Apple Magic Keyboard                                                       |
| Headphones                   | Audio Technica ATX-M50X            | ---                                                                        |

I'm looking to eventually:

- Replace my old Audio Interface with a [Focusrite Scarlett 4i4](https://focusrite.com/usb-audio-interface/scarlett/scarlett-4i4)
- Either reinstall my Corsair H80 Cooler with an AMD AM4 mount, or (if the former isn't possible) switch to the Corsair Hydro Series H55 Cooler as it supports the AM4 mount and I don't feel I need anything bigger than a 120mm radiator for what I'm running on my PC.
- Upgrade my Monitor to a 4K or 5K 27" Monitor (Mmmm, Retina<sup>TM</sup>)

Questions you may have, that I can answer:

- _**What did you do with your old case, components and removed 1TB HDD?**_  
  I've kept it, installed Linux Mint (XFCE4), and will be gifting it to my parents so they can have a free upgrade.  
  If they don't use it/need it, I'll be gifting it to a local charity or good-cause organisation for their use.
- _**Why AMD for your CPU? Why not Intel?**_  
  I do a lot of Software Development, and have lots of things running at once, so I figured the higher Core & Thread count that I get with AMD Ryzen Zen 2 would be beneficial. Plus, with AMD actually competing with Intel on price-v-performance, the 3600X was really good value for what I wanted.
- _**Why AMD for your GPU? Why not nVidia?**_  
  I'd never understood AMD GPU tiers. nVidia is dead easy: GTX = Normal, RTX = Fancy Ray-Tracing, Bigger number = Better. However, I decided that I should try to understand the tiers for AMD.  
  Being a noob, I looked at [this Tom's Hardware Post](https://www.tomshardware.com/uk/reviews/gpu-hierarchy,4388.html) and looked down the list. I didn't want any of the fancy RTX/Ray-Tracing shite, I'd read that AMD had good support for drivers on Linux (nVidia has gotta kinda shitty support), and after watching some LinusTechTips videos on the properties of the various cards, I found that the best price-v-performance product for what I wanted was the AMD Radeon RX 5700.
- _**Why the Apple Magic Keyboard?**_  
  I don't like mechanical keyboards, I like flat keyboards with a small but still noticable travel time. I've tried _loads_ different keyboards, but none beat the keyboard on the Macbook Pro 15" Retina Mid-2015.  
  I spent a bit of time testing the [Apple Magic Keyboard](https://www.apple.com/uk/shop/product/MLA22B/A/magic-keyboard-british-english) and the [Apple Magic Keyboard with Numeric Keypad](https://www.apple.com/uk/shop/product/MRMH2B/A/magic-keyboard-with-numeric-keypad-british-english-space-grey) and found that the _Magic Keyboard_ had, very nearly, the same keyboard feel as the aforementioned Macbook Pro. The _Magic Keyboard with Numeric Keypad_ had a far too "clicky" keyboard feel to it, that I didn't like.
- _**Why do you have Optical Drives & Card Readers in 2019?**_  
  I like playing old games from my childhood, so I have a DVD drive.  
  I want to play Blu-rays on my PC, so I have a Blu-ray drive.  
  I have a DSLR camera and want to support different cards, in case a guest has one of those cards, so I have a Card Reader.  
  For the angry ones amonst you, I'll make it worse: I'll be getting a Floppy Drive Reader soon so I can play the SUPER old games that are currently in my parent's attic.
- _**Why not use your old 120mm fans?**_  
  My new motherboard doesn't support more than 3 chassis fans.

## Detailed View

### CPU

| Detail             | Old                          | New             |
| ------------------ | ---------------------------- | --------------- |
| Make               | Intel                        | AMD             |
| Model              | i5-3570K                     | Ryzen 5 3600X   |
| Brand Generation   | Ivy Bridge (Core i5 3rd Gen) | Zen 2 (3rd Gen) |
| Socket             | LGA 1155                     | AM4             |
| Base Clock         | 3.4GHz                       | 3.8GHz          |
| Cores              | 4                            | 6               |
| L1 Cache           | 256KB                        | 384KB           |
| L2 Cache           | 1.0MB                        | 3MB             |
| L3 Cache           | 6.0MB                        | 32MB            |

### RAM

| Detail      | Old       | New           |
| ----------- | --------- | ------------- |
| Make        | Corsair   | Corsair       |
| Model       | Vengeance | Vengeance LPX |
| DRAM Type   | DDR3      | DDR4          |
| Clock speed | 1333MHz   | 3200MHz       |
| Form Factor | DIMM      | DIMM          |

### Motherboard

| Detail | Old         | New                     |
| ------ | ----------- | ----------------------- |
| Make   | ASUS        | ASUS                    |
| Model  | P8-Z77-V LX | ROG Strix B450-F Gaming |
| Socket | LGA1155     | AM4                     |

### GPU

| Detail             | Old                   | New                |
| ------------------ | --------------------- | ------------------ |
| Make               | EVGA                  | Sapphire           |
| Model              | Nvidia GeForce 780 Ti | AMD Radeon RX 5700 |
| Bus                | PCIe 3.0              | PCIe 4.0           |
| Memory             | 3GB                   | 8GB                |
| Memory Type        | GDDR5                 | GDDR6              |
| Base Memory Clock  | 875MHz                | 1465Mhz            |
| Boost Memory Clock | 928MHz                | 1725Mhz            |

### Sound Card

| Detail        | Removed                                   |
| ------------- | ----------------------------------------- |
| Make          | M-Audio                                   |
| Model         | Delta 66                                  |
| Bus           | PCI                                       |
| Break-out Box | Omni I/O Integrated Desktop Audio Station |

### PSU


| Detail        | Unchanged |
| ------------- | --------- |
| Make          | Corsair   |
| Model         | RM850x    |
| Wattage       | 850W      |

### Storage

SSD #1 - NEW

| Detail    | New          |
| --------- | ------------ |
| Make      | Samsung      |
| Model     | 970 EVO Plus |
| Capacity  | 250GB        |
| NAND Type | MLC          |
| Bus       | M.2          |
| Protocol  | NVMe         |

HDD #1

| Detail     | Unchanged      |
| --------   | -------------- |
| Make       | Seagate        |
| Model      | Barracuda 7200 |
| Capacity   | 2TB            |
| Bus        | SATA           |
| Protocol   | SATA           |
| Spin Speed | 7200rpm        |

HDD #2

| Detail     | Unchanged            |
| ---------- | -------------------- |
| Make       | Western Digital (WD) |
| Model      | Green WD30EZRX       |
| Capacity   | 3TB                  |
| Bus        | SATA                 |
| Protocol   | SATA                 |
| Spin Speed | 7200rpm              |

### CPU Cooling

| Detail        | Old                  | New          |
| ------------- | -------------------- | ------------ |
| Make          | Corsair              | AMD          |
| Model         | H80i                 | Wraith Spire |
| Radiator      | 120mm x 152mm x 38mm | None         |
| Radiator Fans | Corsair 120mm        | None         |

### Tower Cooling

| Detail | Old                  | New                                   |
| ------ | -------------------- | ------------------------------------- |
| Fan #1 | Bitfenix 120mm Merc  | Fractal Design 140mm Silent Series R2 |
| Fan #2 | Corsair 120mm        | Fractal Design 140mm Silent Series R2 |
| Fan #3 | None                 | Fractal Design 140mm Silent Series R2 |

### Optical Drives

Blu-ray Drive #1 - NEW

| Detail      | Unchanged                  |
| ----------- | -------------------------- |
| Make        | LG                         |
| Model       | M-Disc Blu-ray Rewriter    |
| Write Speed | 14x                        |
| Bus         | SATA                       |

DVD Drive #2

| Detail      | Unchanged                  |
| ----------- | -------------------------- |
| Make        | LG                         |
| Model       | M-Disc DVD Rewriter        |
| Write Speed | 24x                        |
| Bus         | SATA                       |

Card Reader #3 - NEW

| Detail      | New                           |
| ----------- | ----------------------------- |
| Make        | KKmoon Sunshine-Tipway (STW)  |
| Model       | STW-3061 Internal Card Reader |
| Bus         | USB 2 & USB 3                 |

### Case

| Detail                   | Old              | New            |
| ------------------------ | ---------------- | -------------- |
| Make                     | Bitfenix         | Fractal Design |
| Model                    | Merc Beta Midi   | Define XL R2   |
| Motherboard Size Support | ATX              | XL-ATX         |
| Colour                   | Black            | Black          |

### Monitors

Main

| Detail     | Unchanged   |
| ---------- | ----------- |
| Make       | BenQ        |
| Model      | GL2450      |
| Size       | 24"         |
| Resolution | 1920 x 1080 |
| Density    | 90ppi       |

Secondary

| Detail     | Removed     |
| ---------- | ----------- |
| Make       | BenQ        |
| Model      | GL2250      |
| Size       | 21.5"       |
| Resolution | 1920 x 1080 |
| Density    | 98ppi       |

### Mouse

| Detail | Old      | New      |
| ------ | -------- | -------- |
| Make   | Maplin   | CSL      |
| Model  | Wireless | SM-800   |

### Keyboard

| Detail | Old      | New            |
| ------ | -------- | -------------- |
| Make   | Maplin   | Apple          |
| Model  | Wireless | Magic Keyboard |

### Headphones

| Detail | Unchanged        |
| ------ | ---------------- |
| Make   | Audio Technica   |
| Model  | ATX-M50X         |
