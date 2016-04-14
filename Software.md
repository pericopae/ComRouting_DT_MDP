This file will change as README.md is updated with concept and feature wishlist.

Quick Steps
-----------

### Required software

- Source management
  - Git for Windows (latest version)
- Build tools
  - Cmake, latest stable version
  - MinGW, version *4.82* 32-bit, the distribution shipped with Qt (QT\Tools\mingw482_32)
  - Visual Studio, VS 2013 (VS 2015 is likely to work, but untested)
- Libraries
  - Required
    - *Qt* >= 5.5.1
        Use the official download from qt.io and the online-installer. It offers
        flexibility in choosing different packages in a single go (e.g. Qt,
        MinGW and Qt Creator) and helps managing maintenance. It provides a
        file structure that accommodates different Qt flavors (Qt built with
        different toolchains), versions, and modules at the same time. We will
        be referring to that file structure throughout this text.

        *Important note*: the flavor of Qt (e.g. msvc2013_64 or mingw492_32) must
        match your toolchain as closely as possible!

        For a 64-bit VS build select msvc2013_64
        for a 32-bit MinGW build select mingw492_32
    - *libsndfile* >= 1.0.25
- Recommended
  - *fftw* >= 3.3.4
  - *readline* >= 5.0 (more recent versions can be found in MinGW distributions)
- Optional
  - *ASIO-SDK* = 2.3 (Asio support in Portaudio)
  - *DirectX SDK* v.7 for MinGW, v.9 for VS. (Direct Sound support in Portaudio)
  - *NSIS*, if you want to create an binary SC installer (add to path)
- Convenience
  - a unix line-ending friendly text editor like *Atom* or *Notepad++*
  - a extraction tool for unixy compression formats like tar and gz, e.g. *7-zip*
