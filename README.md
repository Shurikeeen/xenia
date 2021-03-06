Xenia - Xbox 360 Emulator Research Project
==========================================

Xenia is an experimental emulator for the Xbox 360. For more information see the
[main xenia website](http://xenia.jp/).

Come chat with us about **emulator-related topics** in
[#xenia @ irc.freenode.net](http://webchat.freenode.net?channels=%23xenia&uio=MTE9NzIaa).
For developer chat join `#xenia-dev` but stay on topic. Lurking is fine.
Please check the [frequently asked questions](http://xenia.jp/faq/) page before
asking questions. We've got jobs/lives/etc, so don't expect instant answers.
Discussing illegal activities will get you banned. No warnings.

## Status

Buildbot | Status
-------- | ------
[All](http://build.xenia.jp/waterfall) | [![Build status](http://build.xenia.jp/png?builder=auto-builds)](http://build.xenia.jp/waterfall)
[Windows](https://ci.appveyor.com/project/benvanik/xenia/history) | [![Build status](https://ci.appveyor.com/api/projects/status/ftqiy86kdfawyx3a/branch/master?svg=true)](https://ci.appveyor.com/project/benvanik/xenia/)
[Linux](https://travis-ci.org/benvanik/xenia) | [![Build status](https://travis-ci.org/benvanik/xenia.svg)](https://travis-ci.org/benvanik/xenia)

Some real games run. Most don't.
See the [Game compatibility list](https://github.com/xenia-project/game-compatibility/issues)
for currently tracked games and feel free to contribute your own updates,
screenshots, and information there following the [existing conventions](https://github.com/xenia-project/game-compatibility/blob/master/README.md).

## Disclaimer

The goal of this project is to experiment, research, and educate on the topic
of emulation of modern devices and operating systems. **It is not for enabling
illegal activity**. All information is obtained via reverse engineering of
legally purchased devices and games and information made public on the internet
(you'd be surprised what's indexed on Google...).

## Quickstart

Windows 8.1+ with Python 2.7 and [Visual Studio 2015](https://www.visualstudio.com/downloads/download-visual-studio-vs) and the Windows SDKs installed:

    > git clone https://github.com/benvanik/xenia.git
    > cd xenia
    > xb setup

    # Pull latest changes, rebase, and update submodules and premake:
    > xb pull

    # Build on command line:
    > xb build

    # Run premake and open Visual Studio (run the 'xenia-app' project):
    > xb devenv

    # Run premake to update the sln/vcproj's:
    > xb premake

    # Format code to the style guide:
    > xb format

When fetching updates use `xb pull` to automatically fetch everything and
run premake for project files/etc.

## Building

See [building.md](building.md) for setup and information about the
`xb` script. When writing code, check the [style guide](style_guide.md)
and be sure to run clang-format!

## Contributors Wanted!

**Before contributing code or issues be sure to read [CONTRIBUTING.md](CONTRIBUTING.md).**

Have some spare time, know advanced C++, and want to write an emulator?
Contribute! There's a ton of work that needs to be done, a lot of which
is wide open greenfield fun.

For general rules and guidelines please see [CONTRIBUTING.md](CONTRIBUTING.md).

Fixes and optimizations are always welcome (please!), but in addition to
that there are some major work areas still untouched:

* Help work through missing functionality/bugs in game [compat](https://github.com/benvanik/xenia/issues?labels=compat)
* Add input drivers for [PS4 controllers](https://github.com/benvanik/xenia/issues/60) (or anything else)
* Skilled with Linux? A strong contributor is needed to [help with porting](https://github.com/benvanik/xenia/labels/cross%20platform)

See more projects [good for contributors](https://github.com/benvanik/xenia/issues?labels=good+for+contributors&page=1&state=open). It's a good idea to ask on IRC/the bugs before beginning work
on something.

## FAQ

For more see the main [frequently asked questions](http://xenia.jp/faq/) page.

### Can I get an exe?

Check the [Releases](https://github.com/benvanik/xenia/releases) tab to see
what's there. Updated irregularly.
