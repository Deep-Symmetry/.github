# Component Projects

As described on the [main organization
page](https://github.com/Deep-Symmetry), here are other projects which
feed into the primary ones mentioned above, but are designed to be
usable on their own as well:

* [carabiner](https://github.com/Deep-Symmetry/carabiner) is a small
  C++ program that can be used as a loose bridge to [Ableton
  Link](https://www.ableton.com/en/link/) for people who want to be
  able to synchronize with performances over that protocol.

* [lib-carabiner](https://github.com/Deep-Symmetry/lib-carabiner) is a
  Java library which allows Carabiner to be embedded in a Java
  program, extracting and running the appropriate executable for the
  processor architecture and operating system that is detected.

* [beat-carabiner](https://github.com/Deep-Symmetry/beat-carabiner) is
  a Clojure library that beat-link-trigger uses to synchronize the Pro
  DJ Link player timeline (managed by beat-link) with other
  instruments and software using Ableton Link (managed by
  lib-carabiner).

* [beat-carabiner-java](https://github.com/Deep-Symmetry/beat-carabiner-java)
  is a more recent port of beat-carabiner from Clojure to Java, to
  make that kind of timeline synchronization more easily accessible to
  developers who are not working in Clojure.

* [crate-digger](https://github.com/Deep-Symmetry/crate-digger) is a
  Java library for fetching and parsing rekordbox database exports and
  track analysis files hosted on Pioneer DJ modular music performance
  gear. It is used by beat-link to obtain this information more
  reliably than was previously possible.

* [electro](https://github.com/Deep-Symmetry/electro) is a Java
  library for working with musical time. It is a port of some Clojure
  code in afterglow to give the same capabilities to beat-link and
  beat-carabiner-java without requiring them to embed the Clojure
  runtime.

* [wayang](https://github.com/Deep-Symmetry/wayang) is a Java library
  used by afterglow to display a user interface on the graphical
  display of the Ableton Push 2, and can be used by any other Java
  project that wants to do something similar.

* [ola-clojure](https://github.com/Deep-Symmetry/ola-clojure) is a
  Clojure library making it easier to communicate with the [Open
  Lighting Architecture](https://www.openlighting.org/ola/). It is how
  afterglow communicates with stage lighting.

* [bytefield-svg](https://github.com/Deep-Symmetry/bytefield-svg) is a
  JavaScript node module that provides a Clojure-based domain-specific
  language for creating byte field diagrams. It is used (through
  asciidoctor-bytefield, described next) extensively in creating
  dysentery's reverse-engineering analysis of the Pro DJ Link
  protocol.

* [asciidoctor-bytefield](https://github.com/Deep-Symmetry/asciidoctor-bytefield)
  is a Javascript extension to
  [Asciidoctor.js](https://docs.asciidoctor.org/asciidoctor.js/latest/),
  used to invoke bytefield-svg to create the byte field diagrams in
  the dysentery protocol analysis document (it is used as an extension
  while building the [Antora](https://antora.org) site that presents
  the documentation.

* [graphterglow](https://github.com/Deep-Symmetry/graphterglow) is a
  small Clojure project that is used to build graphs in the afterglow
  documentation showing how beat-related functions vary over time.

## Standalone Projects

There are also a handful of other minor projects which are not
libraries but which you might find useful.

* [open-beat-control](https://github.com/Deep-Symmetry/open-beat-control)
  provides access to a subset of features of beat-link-trigger,
  including tempo bridging between Pro DJ Link networks and Ableton
  Link, using [Open Sound
  Control](https://en.wikipedia.org/wiki/Open_Sound_Control) as a
  limited API. without the requirement of a GUI environment. It can be
  handy if you are already working in an environment (like
  [PureData](https://puredata.info),
  [Max](https://cycling74.com/products/max/), or
  [TouchDesigner](https://derivative.ca)). But there are better
  approaches than OSC if you are not using such an environment, like:

* [java-beat-control-example](https://github.com/Deep-Symmetry/java-beat-control-example)
  is a starter framework for building a Java program that uses
  beat-carabiner-java to interact with both Pro DJ Link networks and
  Ableton Link networks. It provides much of the basic capabilities of
  open-beat-control, and is ready for you to add your own unique
  features using the full power of Deep Symmetry's Java APIs.

* [afterglow-max](https://github.com/Deep-Symmetry/afterglow-max)
  hosts afterglow inside of [Max](https://cycling74.com/products/max/)
  using their Java extension mechanism. Recent releases of Max have
  switch to JavaScript, however, and so are not suitable for such an
  integration.
