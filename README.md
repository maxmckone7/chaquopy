# Chaquopy: the Python SDK for Android
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fmaxmckone7%2Fchaquopy.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fmaxmckone7%2Fchaquopy?ref=badge_shield)


Chaquopy provides everything you need to include Python components in an Android app,
including:

* Full integration with Android Studio's standard Gradle build system.
* Simple APIs for calling Python code from Java/Kotlin, and vice versa.
* A wide range of third-party Python packages, including SciPy, OpenCV, TensorFlow and many
  more.

To get started, see the [documentation](https://chaquo.com/chaquopy/doc/current/).


## Repository layout

This repository contains the following components:

* `product` contains Chaquopy itself.
* `target` contains build processes for Python and its dependencies.
* `server/pypi` contains build processes for third-party Python packages.


## Build

For build instructions, see the README files in each subdirectory.

Or to build everything at once, follow the instructions below on a Linux x86-64 machine:

If necessary, install Docker using the [instructions on its
website](https://docs.docker.com/install/#supported-platforms).

Make sure all submodules are up to date:

    git submodule init && git submodule update

Then run the script `build-maven.sh`. This will generate a `maven` directory containing the
Chaquopy repository.

To use this repository to build an app, edit the `repositories` block in your `settings.gradle`
or `build.gradle` file to [declare your
repository](https://docs.gradle.org/current/userguide/declaring_repositories.html#sec:declaring_multiple_repositories)
before `mavenCentral`. Either an HTTP URL or a local path can be used.


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fmaxmckone7%2Fchaquopy.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fmaxmckone7%2Fchaquopy?ref=badge_large)