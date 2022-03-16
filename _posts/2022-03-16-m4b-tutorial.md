---
layout: post
title:  "Quick audiobook tutorial"
date:   2022-03-16 11:22:22 +0100
categories: tutorial geek
---
How to convert mp3 to a beautiful audiobook?
You need:
1. a **folder** with mp3s tagged (whatever tool, on windows it could be mp3tag.exe)
2. if you want chapter images insert that in tags, each file a different cover
3. add a file cover.jpg to your **folder**, as a main cover of the book
4. get [m4b-tool](https://github.com/sandreas/m4b-tool) as a command-line tool

navigate to your **folder** and run:

    ❯ m4b-tool merge -v "./" --output-file="./audiobook.m4b"

It will scan files, convert them, merge them, maintain tags, add chapter for each file, add cover and everything. This tool has a lot more to offer.