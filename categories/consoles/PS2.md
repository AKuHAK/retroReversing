---
permalink: /ps2
layout: post
title: Sony Playstation 2
recommend: ps2
recommendTitle: All PS2 Posts
editlink: ../categories/consoles/PS2.md
console: 'ps2'
consoleimage: /public/consoles/Sony PlayStation 2.png
thumbnail: /public/consoles/Sony PlayStation 2.png
breadcrumbs:
  - name: Home
    url: /
  - name: Consoles
    url: /
  - name: Sony Playstation 2
    url: #
---

# Hardware
Similar to the original Playstation the PS2 used a MIPS processor but this time it was 64 bit and codenamed the **Emotion Engine**, along with 2 custom vector processors. Although the PS2 has a much more modern GPU design compared to the PS1, the actual transformation of the verticies were still being process by the CPU core rather than the GPU [^1].

The main parts of the PS2 hardware were:
* Emotion Engine (64 bit MIPS processor + 2 vector processors)
* Graphics Synthesiser (GS) - 4MB with features such as Z-buffer, trilinear texturing and gourard shading [^1]
* 48-Channel sound chip (SPU2)

## Retail Hardware
For an in-depth look at the Playstation 2 Retail hardware architecture check out the excellent post by **Copetti.org**:
{% include link-to-other-site.html url="ttps://www.copetti.org/writings/consoles/playstation-2/" description="Copetti.org has an excellent tear down of the Playstation 2 Hardware and how it works" image="https://www.copetti.org/images/consoles/ps2/_hue8a2466eba16e1ae3cd9542d2db31c8a_66348_dcb7ac7ba1db910c9628de3127aa9544.webp" title="Playstation 2 Architecture - A Practical Analysis"  %}


## Development Hardware
The hardware used to develop Playstation 2 games was similar but had an increase in memory along with a few debugging features. The details are covered in a seperate post:
{% include link-to-other-post.html post="/playstation-2-development-hardware" description="For information about Sony's Playstation Two development hardware check out this post." %}

Later in the PS2's lifetime SN Systems released a specific development kit for developing online multiplayer PS2 games compatible with the PS2 Modem called the Network Development Kit (NDK).

{% include link-to-other-post.html post="/sn-systems-network-development-kit-for-ps2/" description="For information about Network Development Kit development hardware check out this post." %}


---
# Games
What would the Sony Playstation 2 be without its excellent line-up of games? It was huge line up of third party the games that attracted many people away from the Nintendo Gamecube and Microsoft Xbox.

## Playstation 2 Games with Debug Symbols
An excellent way to start reverse engineering is to find games where the developers accidentally left the Debug symbols in the retail release of the game. This was surprisingly common in early PS2 games as the SDK didn't remove them when building the final executables. 
These gives you access to all the original function and variables names that were used in the retail source code so are very valuable for reversers!

{% include link-to-other-post.html post="/ps2-unstripped/" description="For a full list of PS2 games that have debug symbols check out this post." %}

## Playstation 2 Demos with Debug Symbols
{% include link-to-other-post.html post="/ps2-demos/" description="For a full list of PS2 games that have debug symbols check out this post." %}

---
# Software Development Kits

## Official Software development kit
The Official Software development kit was developed by a partnership between SN Systems who are known for excellent 3rd party development kits and the Game Studio Psygnosis who are known for excellent quality games.

{% include link-to-other-post.html post="/ps2-official-sdk/" description="For information about Sony's Playstation Two SDK check out this post." %}

### Emotion Engine Static Libraries
The Playstation 2 Software Development kit included various statically compiled libraries that could be optionally included in your games, these ranged from vital (gcc runtime) to optional such as Multi-tap support.

{% include link-to-other-post.html post="/static-libraries-ps2" description="For a list of all the static libraries inside the PS2 SDK check out this post" %}

### Dynamic Libraries (IRX files)
{% include link-to-other-post.html post="/irx-ps2" description="For a list of all the dynamic libraries inside the PS2 SDK and from third parties check out this post" %}

## Consumer Development Kit
Similar to how the PS1 had Net Yaroze for consumers to develop small games for the Playstation, the PS2 had special software that ran a build of Linux. The software ran on consumer PS2 models and came with a PS2 hard-drive.


---
# All Posts
<div>

{% include console.html %}
</div>

---
# References
[^1]: [20 Years of PlayStation®. Console development past and future - Unite Europe 2015 - YouTube](https://www.youtube.com/watch?v=fwCVTqSmioI)
