<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=ffb7d5,b5d8ff,ffd6f5&height=120&section=header" width="100%"/>

```
✦ · · · · · welcome to my github · · · · · ✦
```

# hey, i'm DarThunder <img src="Mv-cinnamon.png" width="35" align="center" />

low-level programmer. i write things close to the metal — C, x86-64 ASM, SIMD, crypto.<br/>
also CC: Tweaked stuff, because why not.<br/>

`I use NixOS btw` &nbsp;·&nbsp; `NixOS on the benchmarks` &nbsp;·&nbsp; `Hyprland enjoyer`

<br/>

[![](https://img.shields.io/badge/C%20%2F%20x86--64%20ASM-ffc2dd?style=flat-square&logoColor=c75591)](https://github.com/DarThunder)
[![](https://img.shields.io/badge/NixOS-d6eeff?style=flat-square&logoColor=2f6fb0)](https://github.com/DarThunder)
[![](https://img.shields.io/badge/low--level%20dev-ece6ff?style=flat-square&logoColor=6b4fc8)](https://github.com/DarThunder)
[![](https://img.shields.io/badge/CC:_Tweaked-d6f5ee?style=flat-square&logoColor=2a8a70)](https://github.com/DarThunder)

</div>

---

## ✦ about me

- I build **low-level systems** — crypto libs, embedded databases, package managers
- Currently obsessed with **hardware-accelerated cryptography** (AES-NI, AVX2, SIMD)
- Studying **side-channel mitigation** and CPU microarchitecture
- Also write Lua for **CC: Tweaked** (Minecraft) because I contain multitudes
- I profile everything. Nanoseconds matter.

---

## ✦ featured project

### [AxiomSSL](https://github.com/DarThunder/AxiomSSL) — high-performance cryptographic library

> built from scratch in C and x86-64 assembly. not for production. very much for understanding.

| Algorithm               | Throughput     | cpb   | Notes                                                |
| ----------------------- | -------------- | ----- | ---------------------------------------------------- |
| AES-ECB (AES-NI + AVX2) | **9,752 MB/s** | 0.205 | 12x block unrolling, saturates Zen 2 pipeline        |
| AES-CTR (AES-NI + AVX2) | **7,904 MB/s** | 0.253 | parallel counter blocks + AVX2 XOR                   |
| AES-CBC (AES-NI)        | 1,445 MB/s     | 1.38  | inherently serial — measures raw HW latency          |
| ChaCha20 (SSE)          | 544 MB/s       | 3.67  | 1-block xmm; AVX2 4-block planned                    |
| SHA-256 (scalar C)      | 266 MB/s       | 7.50  | optimized scalar baseline                            |
| SM4 (masked S-Boxes)    | 98 MB/s        | 20.33 | side-channel mitigation costs performance, by design |

benchmarks run on AMD Ryzen 5 5500U · 2047 MB buffer · 20 iterations · outliers filtered · `rdtsc` + `mfence` + `cpuid` barriers

---

## ✦ stack

**systems & low-level**

![C](https://img.shields.io/badge/C-ffc2dd?style=flat-square)
![Assembly x86-64](https://img.shields.io/badge/Assembly%20x86--64-d6eeff?style=flat-square)
![Lua](https://img.shields.io/badge/Lua-ece6ff?style=flat-square)
![Java](https://img.shields.io/badge/Java-ffd6ec?style=flat-square)
![Make](https://img.shields.io/badge/Make-d6f5ee?style=flat-square)

**tools & env**

![Arch Linux](https://img.shields.io/badge/Arch%20Linux-d6eeff?style=flat-square)
![NixOS](https://img.shields.io/badge/NixOS-e8eeff?style=flat-square)
![Hyprland](https://img.shields.io/badge/Hyprland-fce8ff?style=flat-square)
![GCC](https://img.shields.io/badge/GCC-d6f5ee?style=flat-square)
![perf](https://img.shields.io/badge/perf-fff3e0?style=flat-square)
![Git](https://img.shields.io/badge/Git-fff0e8?style=flat-square)

---

## ✦ github stats

<div align="center">

[![GitHub stats](https://github-readme-stats-one-bice.vercel.app/api?username=DarThunder&show_icons=true&theme=rose_pine&hide_border=true&bg_color=fff0f5&title_color=c75591&icon_color=5b9bd5&text_color=6a4a6a&ring_color=ffc2dd)](https://github.com/DarThunder)

[![Top Langs](https://github-readme-stats-one-bice.vercel.app/api/top-langs/?username=DarThunder&layout=compact&hide=html,css,javascript&theme=rose_pine&hide_border=true&bg_color=fff0f5&title_color=c75591&text_color=6a4a6a)](https://github.com/DarThunder)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=ffb7d5,b5d8ff,ffd6f5&height=80&section=footer" width="100%"/>

_made with ♡ and questionable amounts of assembly_

</div>
