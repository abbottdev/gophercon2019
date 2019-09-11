# Gio

Cross Platform GUI Programming for Mobile, Desktop, WebAssembly


## Speaker

Elias Naur [@elias_naur](https://twitter.com/elias_naur)

Elias is a long-time maintainer of the iOS and Android Go runtime, and until recently the maintainer of Go Mobile.

## Intro

Gio is a new open source Go library for writing immediate mode GUI programs that run on all the major platforms: Android, iOS/tvOS, macOS, Linux, Windows and WebAssembly. The talk will cover Gio’s unusual design and how it achieves simplicity, portability and performance.

## Resources

[Slides](https://go-talks.appspot.com/github.com/eliasnaur/gophercon-uk-2019-talk/gophercon-uk-2019-live.slide#1)
[Code](https://github.com/eliasnaur/gophercon-uk-2019-talk)
[Video Recording](https://www.youtube.com/watch?v=9D6eWP4peYM)

Notes: Elias Naur presented Gio, a new open source Go library for writing immediate mode GUI programs that run on all the major platforms: Android, iOS/tvOS, macOS, Linux, Windows. The talk covered Gio’s unusual design and how it achieves simplicity, portability and performance.

Elias said, “I wanted to be able to write a GUI program in GO that I could implement only once and have it work on every platform. This, to me, is the most interesting feature of Gio.”

Elias also presented Scatter which is a Gio program for end-to-end encrypted messaging over email.

Other features of Gio include:

- Immediate mode design
- UI state owned by program
- Only depends on lowest-level platform libraries
- Minimal dependency tree to keep things low level as possible
- GPU accelerated vector and text rendering
- It’s super efficient
- No garbage generated in drawing or layout code
- Cross platform (macOS, Linux, Windows, Android, iOS, tvOS, Webassembly)
- Core is 100% Go while OS-specific native interfaces are optional