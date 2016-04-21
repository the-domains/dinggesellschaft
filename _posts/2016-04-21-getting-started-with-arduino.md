---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
starred: false
keywords: []
description: "Arduino is cheap embedded platform based on the Atmel. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the Arduino are NeoVim, platformio and GNU Make."
datePublished: '2016-04-21T15:08:37.386Z'
dateModified: '2016-04-21T15:07:48.849Z'
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

[Arduino][0] is cheap embedded platform based on the [Atmel][1]. It's good to build devices for analog sensoring, controlling electric devices or even build robots. The tools I use to program the [Arduino][0] are [NeoVim][2], [platformio][3] and [GNU Make][4].

## About the editor

Sure you can use the IDE of [http://arduino.cc][0] or [http://arduino.com][5], they are quiet equal, but you will get soon to the limits. I prefer [Vim][6] or the newer implementation [NeoVim][7], with a few plugins like [syntastic][8], [deoplete][9] and [clang\_complete][10]. [Syntastic][8] helps to keep the syntax clean, [deoplete][9] and [clang\_complete][10] providing autocompletion.

## About the toolchain

When it comes to compiling, I use [platformio][3]. It's a command line tool which can handle multiple tasks which makes life much more comfortable for me.

First feature I like is you can create environments, which control for which device you want to compile for and setting compiler flags. The important compiler flags already setted by the environment, but you can add your own which gives you the chance to fine tune your build and your compiler.

The second feature is that you can search, add, remove and update libraries. [Platformio][3] provides a [web service][11] for that where a whole bunch of libraries are registered.

The possibility to build, upload and connect via serial are given, so you have all required tools in one place.

## Make life even more simple

[GNU Make][4] is one of the most used build systems in FOSS world. I usally write a makefile with targets for every environment. I also write targets for testing and uploading to have shortcuts for this jobs.

The good thing of this is that it integrates great into [Vim][6] and [NeoVim][2].

## Conclusion

I have a small toolset to develop, build and debug with the [Arduino][0] platform. I can concentrate to the things I want to do and I can create complex systems without any problems.

[0]: http://arduino.cc/
[1]: http://www.atmel.com/
[2]: http://neovim.io/
[3]: http://platformio.org/
[4]: http://www.gnu.org/software/make/
[5]: http://arduino.com/
[6]: http://www.vim.org/
[7]: https://neovim.io/
[8]: https://github.com/scrooloose/syntastic
[9]: https://github.com/Shougo/deoplete.nvim
[10]: https://github.com/Rip-Rip/clang_complete
[11]: http://platformio.org/lib