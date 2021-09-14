---
layout: post
title: IDA Pattern Search - Using bitfield patterns to identify functions in binaries
---

Many security researchers have a monogamous relationship with IDA Pro. I get it, IDA Pro is a powerful tool and has beautiful color schemes, but that doesn’t mean other disassemblers don’t have amazing features that you simply can’t find in IDA. Take for example Ghidra, which offers awesome perks when analyzing raw embedded firmware. One of these perks is the ability to efficiently locate functions using bit-patterns, according to the CPU architecture - a challenge my colleagues and I often tackle on the Argus research team. Since I miserably failed to convince them to give Ghidra a chance, I implemented this Ghidra feature on IDA (borrowing Ghidra’s format for bit-patterns). 

I’m sharing this tool on GitHub ([IDAPatternSearch](https://github.com/david-lazar/IDAPatternSearch)) and the full blog post is published in [Argus blog](https://argus-sec.com/using-bitfield-patterns-to-identify-functions-in-binaries/) where I’ll explain Ghidra's format for bit-patterns, how to generate new patterns and how to use the introduced tool. Hope you’ll find it useful!
