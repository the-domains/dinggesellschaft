---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
starred: false
keywords: []
description: "Arduino is cheap embedded platform based on the Atmel. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the Arduino are NeoVim, platformio and GNU Make."
datePublished: '2016-04-21T14:44:56.278Z'
dateModified: '2016-04-21T14:44:55.339Z'
title: Getting started with Arduino
author: []
authors: []
publisher:
  name: null
  domain: null
  url: null
  favicon: null
sourcePath: _posts/2016-04-21-getting-started-with-arduino.md
published: true
url: getting-started-with-arduino/index.html
_type: Article

---
# Getting started with Arduino

Arduino is cheap embedded platform based on the Atmel. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the Arduino are NeoVim, platformio and [GNU Make][0].

## About the editor

Sure you can use the IDE of [http://arduino.cc][1] or [http://arduino.com][2], they are quiet equal, but you will get soon to the limits. I prefer [Vim][3] or the newer implementation [NeoVim][4] with a few plugins like [syntastic][5], [deoplete][6] and [clang\_complete][7]. [Syntastic][5] helps to keep the syntax clean, [deoplete][6] and [clang\_complete][7] providing autocompletion.

## About the toolchain

When it comes to compiling, I use [platformio][8]. It's a command line tool which can handle multiple tasks which makes life much more comfortable for me.

First feature I like is you can create environments, which control for which device you want to compile for and setting compiler flags. The important compiler flags already setted by the environment, but you can add your own which gives you the chance to fine tune your build and your compiler.

The second feature is that you can search, add, remove and update libraries. Platformio provides a web service for that where a whole bunch of libraries are registered.

The possibility to build, upload and connect via serial are given, so you have all required tools in one place.

## Make life even more simple

[GNU Make][0] is one of the most used build systems in FOSS world. I usally write a makefile with targets for every environment. I also write targets for testing and uploading to have shortcuts for this jobs.

The good thing of this is that it integrates great into [Vim][3] and [NeoVim][9].

## Conclusion

I have a small toolset to develop, build and debug with the Arduino platform. I can concentrate to the things I want to do and I can create complex systems without any problems.

[0]: http://www.gnu.org/software/make/
[1]: http://arduino.cc/
[2]: http://arduino.com/
[3]: http://www.vim.org/
[4]: https://neovim.io/
[5]: https://github.com/scrooloose/syntastic
[6]: https://github.com/Shougo/deoplete.nvim
[7]: https://github.com/Rip-Rip/clang_complete
[8]: http://platformio.org/
[9]: http://neovim.io/