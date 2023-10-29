## Component Projects

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

* [beat-carabiner][https://github.com/Deep-Symmetry/beat-carabiner] is
  a Clojure library that beat-link-trigger uses to synchronize the Pro
  DJ Link player timeline (managed by beat-link) with other
  instruments and software using Ableton Link (managed by
  lib-carabiner).

* [beat-carabiner-java](https://github.com/Deep-Symmetry/beat-carabiner-java)
  is a more recent port of beat-carabiner from Clojure to Java, to
  make that kind of timeline synchronization more easily accessible to
  developers who are not working in Clojure.
