# retrobuild

A build tool for retro consoles & retro computers

## Goals
- Provide full build of cross toolchains & dependencies
- Build from code to ROM & other formats
  - e.g., with layering the build, we could bundle outputs with emulators
- If/when flashing or other tools or required, try to download, build or provide those, too.
  - Be able to build or download any free replacement fw or Operating Systems
    - e.g., EmuTOS
- Offer build options & pluggable toolchains
  - e.g. use different assemblers with different options
  - have debug builds, distribution builds, etc
- Try to work across Linux, Windows & macOS, at least or try to at least degrade gracefully
- More TBD

## NonGoals
- To be any kind of product or compete with emulators or anything else
  - Instead, we would want emulator authors to think our tools were useful
- We can't get too bogged down with subtly fixing any/all dependencies if they don't work on a certain platform
- We will not be distributing emulators or bzlmods for emulators
- IDEs or IDE plugins
  - We want to be an IDE-agnostic build tool that is useful to all sorts of retro developers, hackers & hobbyists
- Package Manager or package management
  - We do not want to mess with your system packages or installation: wherever possible we will build static binaries from source for our toolchains & toolchain dependencies. emulators/simulators and other tools will be installed into an output/ sandbox directory.
  - If any system installations are ever needed, we will separate them from the rest of the build so that the user can decide how to do them.
- More TBD 
