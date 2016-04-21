---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
starred: false
keywords: []
description: "Arduino is cheap embedded platform based on the Atmel. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the Arduino are NeoVim, platformio and GNU Make."
datePublished: '2016-04-21T15:04:40.614Z'
dateModified: '2016-04-21T15:02:42.543Z'
title: Getting started with Arduino
author: []
sourcePath: _posts/2016-04-21-getting-started-with-arduino.md
published: true
authors: []
publisher:
  name: null
  domain: null
  url: null
  favicon: null
url: getting-started-with-arduino/index.html
_type: Article

---
# Getting started with Arduino

Arduino is cheap embedded platform based on the Atmel. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the [Arduino][0] are [NeoVim][1], [platformio][2] and [GNU Make][3].

## About the editor

Sure you can use the IDE of [http://arduino.cc][0] or [http://arduino.com][4], they are quiet equal, but you will get soon to the limits. I prefer [Vim][5] or the newer implementation [NeoVim][6], with a few plugins like [syntastic][7], [deoplete][8] and [clang\_complete][9]. [Syntastic][7] helps to keep the syntax clean, [deoplete][8] and [clang\_complete][9] providing autocompletion.

## About the toolchain

When it comes to compiling, I use [platformio][2]. It's a command line tool which can handle multiple tasks which makes life much more comfortable for me.

First feature I like is you can create environments, which control for which device you want to compile for and setting compiler flags. The important compiler flags already setted by the environment, but you can add your own which gives you the chance to fine tune your build and your compiler.

The second feature is that you can search, add, remove and update libraries. Platformio provides a web service for that where a whole bunch of libraries are registered.

The possibility to build, upload and connect via serial are given, so you have all required tools in one place.

## Make life even more simple

[GNU Make][3] is one of the most used build systems in FOSS world. I usally write a makefile with targets for every environment. I also write targets for testing and uploading to have shortcuts for this jobs.

The good thing of this is that it integrates great into [Vim][5] and [NeoVim][1].

## Conclusion

I have a small toolset to develop, build and debug with the Arduino platform. I can concentrate to the things I want to do and I can create complex systems without any problems.

[0]: http://arduino.cc/
[1]: http://neovim.io/
[2]: http://platformio.org/
[3]: http://www.gnu.org/software/make/
[4]: http://arduino.com/
[5]: http://www.vim.org/
[6]: https://neovim.io/
[7]: https://github.com/scrooloose/syntastic
[8]: https://github.com/Shougo/deoplete.nvim
[9]: https://github.com/Rip-Rip/clang_complete