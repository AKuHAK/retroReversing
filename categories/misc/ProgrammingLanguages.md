---
layout: post
permalink: /programming-languages
thumbnail: /public/images/RetroReversingLogoSmall.png
console: programming
breadcrumbs:
  - name: Home
    url: /
redirect_from:
  - /languages
editlink: '../categories/misc/ProgrammingLanguages.md'
title: Exploring Retro Game Programming Languages - From Assembly to higher level languages
recommend: 
 - programming
 - software
tags:
 - programming
---

# Introduction
Welcome to our journey through the fascinating world of programming lanugaes used to create retro games! 
In the early days of video games, developers had to work with limited resources and hardware, pushing the boundaries of creativity and innovation. 
One of the crucial aspects of game development during that era was the choice of programming language. 
In this article, we'll delve into some of the most iconic languages used in creating retro games, from the low-level intricacies of Assembly to the user-friendly environments of more modern programming languages.

# Assembly Language (z80/6502/68000/x86/arm/sh2)
Assembly language is as low-level as it gets, offering direct control over a computer's hardware. 
In the realm of retro game development, Assembly was the language of choice for squeezing every last drop of performance from early gaming consoles and home computers. 
While notoriously difficult to master, it provided unparalleled speed and efficiency, making it ideal for crafting games that pushed hardware limits to the edge.

However assembly language programs are written fro a specific CPU and not portable to different CPU architectures.

Mosy commercial games written for Game Boy/Game Boy Color/NES/SNES/SMS/MegaDrive are written in an Assembly language such as z80/6502/68000 as C compilers were generally not good enough at the time to create optimized code for those platforms.

---
# C/C++
C and C++ revolutionized game development by introducing a higher level of abstraction without sacrificing performance (when compilers became good enough between the Mega Drive and Saturn era). 
Their versatility and efficiency allowed developers to create complex gameplay mechanics and stunning visuals while maintaining compatibility with a wide range of platforms.

Most games post MegaDrive/SNES/Game Boy Color were written in C and many games post PS1 were written in C++.

However there are some interesting exceptions to this rule such as commercial Game Boy Color games written in C (e.g Lego Stunt Rally [^2], Datel Rocket games).

Also there is one known commerical Mega Drive game to be written in C, **Sonic Spinball** [^5]!

One good way to tell if a game uses C/C++ is to look for C-style strings in the disassembed code/memory.

---
# Basic Variants
With Assembly having a reputation for being difficult to learn, many "simpler" programming languages were created with one of the most popular earlier languages simply being called "BASIC".
Over the years many Badic varients were released tailored for hobbiest game programmers.

## Blitz Basic
Blitz Basic emerged as a game-changer for aspiring Amiga game developers in the 1990s. 
With its simplified syntax and built-in libraries, Blitz Basic empowered enthusiasts to create games without the steep learning curve associated with traditional programming languages. 
Its user-friendly interface and rapid development capabilities made it a popular choice for hobbyists and indie developers looking to bring their retro game ideas to life.

Popular games made using Blitz Basic:
* **Super Skidmarks** - Amiga
* **Worms** - Amiga

BlitzBasic later evolved into **Blitz2D** which was for creating games for DOS/Windows and has continued to evolve into future products such as **Blitz3D** [^1].

## Dark Basic
Dark Basic, a more modern version of Amiga tools such as Blitz Basic or AMOS, took simplicity to the next level by focusing specifically on game development. 
Tailored for beginners and hobbyists, it provided a robust set of tools for creating 2D and 3D games with ease. Dark Basic's intuitive scripting language allowed developers to concentrate on game design without getting bogged down in technical details, making it an accessible gateway to the world of game development for hobbiest.

However no popular commercial AAA games were ever developed with Dark Basic as far as we can see, a few multimedia applications were created using Dark Basic:
* **The 3D Game Maker** which was also written by the creators of Dark Basic (TheGameCreators) and sold reasonably well.
* **Driving Test Success Practical** by Focus which sold over 100k units [^3]

Dark Basic Professional was later released which was re-written from scratch and allowed plugins to be developed to extend the functionality.

The FPS Creator (also by TheGameCreators) was written in Dark Basic Professional and its source code is now available on Github [^4].

You can find the full source code to Dark Basic Professional including the compiler on github: [TheGameCreators/Dark-Basic-Pro: Dark Basic Pro is an open source BASIC programming language for creating Windows applications and games](https://github.com/TheGameCreators/Dark-Basic-Pro)

You can find out more about all TheGameCreators products in this excellent documentary from **TannerProductions**:
<iframe width="560" height="315" src="https://www.youtube.com/embed/H74kuD1g1wg?si=tnyV7nPXcb_MglSN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
# References
[^1]: [Scripting language: Blitz Basic - MobyGames](https://www.mobygames.com/group/11091/scripting-language-blitz-basic/)
[^2]: [Quang Nguyen - Nintendo Game Boy Development - Media - Computing History](https://www.computinghistory.org.uk/det/56957/Quang-Nguyen-Nintendo-Game-Boy-Development/)
[^3]: [The Game Creators Newsletter - Issue 50](https://www.thegamecreators.com/pages/newsletters/newsletter_issue_50.html)
[^4]: [FPS-Creator-Classic/Dark Basic Pro Shared/Dark Basic Pro/Projects/FPSCREATOR at master · TheGameCreators/FPS-Creator-Classic](https://github.com/TheGameCreators/FPS-Creator-Classic/tree/master/Dark%20Basic%20Pro%20Shared/Dark%20Basic%20Pro/Projects/FPSCREATOR)
[^5]: [Interview: Peter Morawiec (2007-04-20) by Sega-16 - Sega Retro](https://segaretro.org/Interview:_Peter_Morawiec_(2007-04-20)_by_Sega-16?rdfrom=https%3A%2F%2Finfo.sonicretro.org%2Findex.php%3Ftitle%3DInterview%3A_Peter_Morawiec_%282007-04-20%29_by_Sega-16%26redirect%3Dno)
