---
layout: single
title: "Charybdis: Keyboard with Trackball"
excerpt: "Motivation, build log and notes for the crystal Charybdis Ergonomic Mechanical Keyboard with Trackball"
header:
  teaser: assets/projects/charybdis_build/showcase/main.jpg
tags:
    - Mechanical Keyboard
    - DIY
    - Ergonomy
    - Productivity
    - Keeb
    - Charybdis
toc: true
toc_sticky: true
author_profile: true
classes: wide
---

# Short version

This write up will focus on the points and showcasing the final result.

## Showcase

<figure class="one">
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
</figure>
<figure class="half">
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
</figure>
<figure class="third">
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
    <a href="/assets/projects/charybdis_build/showcase/main.jpg"><img src="/assets/projects/charybdis_build/showcase/main.jpg"></a>
</figure>

## Specifications

**Model:** [Charybdis 4x6](https://bastardkb.com/charybdis/)

**Case:**: 3D printed with Formalabs 3B, Clear Resin v4, Custom Engraving (**TODO** Add link to section)

**Switches:**: Kaihl Pro Purple x 56

**Keycaps:** Blank transluescent DSA key caps

**Other:**

- Trackball with 3D printed BTU instead of the default bearings
- RGB key back-light
- Hot swap for key switches
- Socketed Elite-C micro-controller (MCU)


## Benefits

- The abandon of the staggered key layout toward _columnar_ or _staggered ortholinear_ (such as ErgoDash too) is a net positive. Charybdis brings this aspect one step further by adding depths to match the different lengths of each finger.
- Split keyboard allows for healthier and more comfortable posture.
- Thumb cluster leverages the thumb for better efficiency.
- Frees up some real estate on the desk, makes it more flexible.
- The use of tenting greatly reduces pronation and the pain associated with it, further improving comfort and efficiency.
- Freedom to customize the keyboard layout to fit specific use case, which can bring non-negligible quality of life improvements.
- Compared to the previous [ErgoDash build](/projects/2020-08-ergodash-build/), Charybdis' trackball combined with an even more reduced key count and the leverage of layers drastically reduces hand movement, thus further improving comfort and efficiency.

## Caveats

- Pricey. With a base price of around 400\\$ (probably), it can go higher depending on the kind of components one decides to use. This specific builds amount to 720\\$, and that is without accounting for the 3D printing machine used to print the case, and the soldering tools.
- Requires some technical skill (electronics assembly and soldering, diagnosing assembly problem, etc...). Compared to ErgoDash, the Charybdis has a higher difficulty namely due to the presence of a trackball and flexible PCB mounting (especially if doing a hot-swap key switch build).
- For someone that has gotten used to standard _staggered_ keyboard layouts, a learning curve for the improved layout. This barely passes as a caveats, as the comfort of using an ergonomic keyboard vastly makes up for it in the medium to long-term.
- _Once you try it, you will never want to come back_. In case one has to work at different physical locations, the high price and time investment makes having duplicate configuration prohibitive. While proficiency with standard keyboard will hardly be affected, it becomes very unpleasant to do so. In my personal case, having to use a standard case leads to unending rants and bout of annoying _ergo keyboard master race elitism_ that probably annoys the people around. Using laptop keyboards also becomes a similarly unpleasant (and potentially painful) activity.

## Important build notes

**TODO** particularly difficult things related to this build.

- For a clear build, manual positioning of the printing support to optimise the aesthetics might be better than automatically generated.
- When doing a hot-swapper key switches build, depending on how tight the hot-swap sockets are can lead to flexible PCB *sliding off* the key switches' pin.
- 

# Build notes (Long version)

## Motivation

Around two years ago, I entered the world of custom ergonomic keyboards with the [ErgoDash build](/projects/2020-08-ergodash-build/).
While this was decently balanced build in terms of difficulty and features, there was mainly two shortcomings that kept on nagging over the years, slowly building the impetus to move on to the Charybdis.

First, despite its ergonomic nature, there was still a need to move the right hand to reach for the mouse.
Having a workflow that sometimes requires prolonged use of the mouse, this quickly become as source of discomfort.
Second, the tenting solution was not as flexible, nor as high enough as I would have expected to have be optimally comfortable.

Although the two shortcoming above were decently solved by having a [trackball slid just right under the tented right case](/projects/2020-08-ergodash-build/#cons), both components being detached would sometimes make it difficult to move then reposition the keyboard and mouse to the optimal location on the desk.
Furthermore, the trackball would sometimes slid too far under the case, resulting in the latter pushing on the "Previous" or "Next" key of the former. This would result in erratic behavior of the computer especially when using a web browser, as well as the inability to input any character.

The *need* more *compact* design that combined both the ergonomics of the ErgoDash as well as the trackball slowly crept up overtime.
As I was lurking in [r/ErgoMechKeyboards](https://reddit.com/r/ergomechkeyboards) and various ergonomic keyboards websites and discord servers, the Charybdis caught might attention for its convenient sourcing (can order all the necessary part in one go), a further fleshed out *2.5D columnar key layout* that looked much more ergonomical, and an easy to install trackball.
While I originally started the Charybdis build to introduce a lab colleague to DIY ergonomic keyboards, a hands on trial with the finished product was the final impetus toward finally building one for myself.

Also, these few paragraphs are probably more of a justification to myself for spending a non-negligible amount of money, time, and effort to build this board.

## Part List

The following is the list of the various parts and components to source, with an approximate on the price as of May 2022 for reference.
The components to order might vary depending on the degree of customization might desired (different 3D case printing ? different key switches ? with or without hot-swap / micro-controller socketing ? etc...).
But in that case, the following part list should at best serve as a vague reference.

moreover, depending on the builder's geographical location, there might be better offers or method of acquisition for those various parts.

| Part and quantity                                                                            | Core build   | Case 3D print | Key hot-swap / MCU socketing **[Optional]** |   Price   |
| :-----------------------------------------------------------------------------------------   | :----------: | :-----------: | :--------------------------: |  -------: | 
| [Charybdis electronics kit: Base kit + Per key RBG + Elite C $\times$ 2 + Trackball](https://bastardkb.com/product/charybdis-electronics-kit/) (1)   |      ✓       |               |                              |  ~\\$270  |
| Blank transluescent DSA keycaps $\times$ 56 [Yusha Kobo](https://shop.yushakobo.jp/en/collections/keycaps/products/dsa-blank-keycaps?variant=37665598308513) [Talp Keybaord](https://talpkeyboard.net/items/5d6e2a6ed0f2564e25201388)                                              |      ✓       |               |                              |  ~\\$45   |
| [Kaihl Pro Purple](https://shop.yushakobo.jp/en/collections/all-switches/products/kailh-pro?variant=37665714700449) $\times$ 56                                                             |      ✓       |               |                              |  ~\\$41   |
| TRRS Cable $\times$ 1 (2)                                                                        |      ✓       |               |                              |  ~\\$10   |
| USB Type C-to-A $\times$ 1 (2)                                                                   |      ✓       |               |                              |  ~\\$9    |
| 6L IPA for 3D prints cleaning  (2)                                                               |              |       ✓       |                              |  ~\\$26   |
| [FormLabs Resin Clear v4](https://formlabs.com/store/clear-resin/)                                                                  |              |       ✓       |                              |  ~\\$150  |
| [Clear UV Cut Coating](https://www.amazon.co.jp/GSI%E3%82%AF%E3%83%AC%E3%82%AA%E3%82%B9-Mr-%E3%82%B9%E3%83%BC%E3%83%91%E3%83%BC%E3%82%AF%E3%83%AA%E3%82%A2%E3%83%BC-UV%E3%82%AB%E3%83%83%E3%83%88-%E3%83%9B%E3%83%93%E3%83%BC%E7%94%A8%E4%BB%95%E4%B8%8A%E6%9D%90-B522/dp/B002DTL7Y4/ref=sr_1_1?__mk_ja_JP=%E3%82%AB%E3%82%BF%E3%82%AB%E3%83%8A&crid=13JXWXNBA6D7N&keywords=clear+uv+cut+coating&qid=1653307061&sprefix=clear+uv+cut+coatin%2Caps%2C202&sr=8-1) $\times$ 2                                                          |              |       ✓       |                              |  ~\\$10   |
| [Sand paper for 3D print polish](https://www.amazon.co.jp/Aewio-%E8%80%90%E6%B0%B4-%E9%AB%98%E7%B4%9A%E3%81%AA%E3%82%B5%E3%83%B3%E3%83%89%E3%83%9A%E3%83%BC%E3%83%91%E3%83%BC-1000-30%E6%9E%9A%E3%82%BB%E3%83%83%E3%83%88/dp/B08242YS2H/ref=sr_1_32_sspa?__mk_ja_JP=%E3%82%AB%E3%82%BF%E3%82%AB%E3%83%8A&crid=2PSNESBOH2Z8T&keywords=sand%2Bpaper%2Bpolish&qid=1653308227&sprefix=sand%2Bpaper%2Bpolis%2Caps%2C202&sr=8-32-spons&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUExR1pTQTBXSURBTExEJmVuY3J5cHRlZElkPUEwMjc5MDk1MVkzWENXM1VWSU1SQSZlbmNyeXB0ZWRBZElkPUEzQ1BMSVMwTE4zTEYwJndpZGdldE5hbWU9c3BfbXRmJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ&th=1)                                                           |              |       ✓       |                              |           |
| [Mill-Max 0305 Holtite for Switches - Hotswap Sockets](https://keycapsss.com/keyboard-parts/parts/73/mill-max-0305-holtite-for-switches-hotswap-sockets?number=KC10042_50x) $\times$ 100 (3)                    |              |               |              ✓               |  ~\\$18   |
| [MCU header sockets + 24 pins](https://keycapsss.com/keyboard-parts/parts/100/single-row-socket-headers-or-pins-mill-max-series-315?number=KC10067_pins) $\times$ 2                                                  |              |               |              ✓               |  ~\\$22   |
| Other fees (4)                                                                               |      -       |       -       |              -               |  ~\\$60   |
| Total                                                                                        |              |               |                              |  ~\\$661  |

**Notes**
- (1): The case is not included. One might print their own case, or also purchase it directly from the website as a different kit. There is also a "Prebuilt" option.
- (2): General enough products that do not warrant a link ... unless one might be interested in also [DIY-ing the cables](https://www.zapcables.com/).
- (3): Already having some from the previous build, so 100 were enough. Strictly speaking however, one would need to order $56 \times 2$ thus $112$ to have enough for all the keys.
- (4): Depending on the geographical location, not only the prices part, but also the import tax, various other taxes, and shipping fees can add up to a non-negligible amount.

## Building steps

Rigorously, the [**Charybdis**](https://bastardkb.com/charybdis/) refers to the side of the board that holds the trackball, while the other side is a [**Scylla**](https://bastardkb.com/scylla/) board, which does not have a trackball.
In this build, the left side uses the **Scylla** board, while the right side uses the **Charybdis** with the trackball.

__TODO__: Forget not the disclaimer that this is not an official build order, but just the commitment of my build experience.
Also insist on the difference with the standard build: hot-swapping, elite-c socketing, custom 3D printing and engraving.

- As it was the first time building such a keyboard, it might be safer to start with the *Scylla* sides that is relatively simpler, owing to the lack of trackball.

### 1. 3D printing the cases [Optional] [Left, Right]

**TODO**: Have we mentioned to make sure that before printing the case, to make sure that it is the correct orientation (left or right).

- Bonus: the STL files for the hand rest.

### 2. Installing the diodes [Left, Right]

### 3. Installing the RGB components [Optional] [Left, Right]

### 4. Installing Mill-Max sockets for hot-swap [Optional] [Left, Right]

### 5. Ribbon cables and RGB cables [Left, Right]

### 6. Installing the Elite-C MCU [Left, Right]

### 6.5 Installing the trackball sensor [Right side only]

### 7. Assembling the case [Left, Right]

## Key layout and firmware 

- Expand on the rational behind the layout design
- Add the steps for flashing.
__NOTE / TODO__ By this point, you should have already cloned the bkb-master branch, consolidated the qmk firmware under a single repository for both j0554 and dosssman, and describe the clean process of installing it.

Consider cloning and zipping the github repositories files themselves, host them and add them to the post  as a form of backup ?

# Acknowledgment
- Sir Quentin
- The BKB community, and more generally, the open source community.
- Professor Takiguchi for the 3D printing machine setup
- Jojo-san for the pictures / help building. **TODO** Any link to a public page ?
- The willpower required for months long saving up of money.
