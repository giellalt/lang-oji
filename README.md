The Ojibwa morphology and tools
===============================

[![GitHub issues](https://img.shields.io/github/issues-raw/giellalt/lang-oji)](https://github.com/giellalt/lang-oji/issues)
[![Build Status](https://github.com/giellalt/lang-oji/workflows/Speller%20CI+CD/badge.svg)](https://github.com/giellalt/lang-oji/actions)
[![License](https://img.shields.io/github/license/giellalt/lang-oji)](https://github.com/giellalt/lang-oji/blob/main/LICENSE)

NOTE: DEVELOPMENT IN OJI HAS BEEN SUSPENDED (03/29/2016) TEMPORARILY IN
FAVOR OF OTW. CURRENT MATERIALS ARE APPROPRIATE FOR NON-NORTHERN
DIALECTS (LEXICON AND MORPHOLOGY), AND THERE HAS BEEN SOME WORK
DEDICATED TO MAKING MORPHOPHONOLOGY FOR THE SYNCOPATED EASTERN DIALECTS.
A \"GLOSSING\" APPROACH HAS BEEN TAKEN TOWARDS THE MORPHOLOGY, AND WORK
HAS BEEN DONE TOWARDS TRANSLATING THAT TO INTO MORE ABSTRACT TAGS. OTW
HAS FULLER VERSIONS OF PHONOLOGY, MORPHOLOGY, TAG ABSTRACTION, AND AN
OTW-SPECIFIC LEXICON.

This directory contains source files for the Ojibwa language morphology
and dictionary. The data and implementation are licenced under the __LICENSE__
licence, also detailed in the
[LICENSE](https://github.com/giellalt/lang-oji/blob/main/LICENSE). The
authors named in the AUTHORS file are available to grant other licencing
choices.

Install proofing tools and [keyboards](https://github.com/giellalt/keyboard-oji)
for the Ojibwa language by using the [Divvun Installer](http://divvun.no)

Documentation
-------------

Documentation can be found here:

- [In source documentation generated with github
   pages](https://gilellalt.github.io/lang-oji/)
-   <https://giellalt.uit.no/lang/oji/OjibwaDocumentation.html>
    (analyser)
-   <https://giellalt.uit.no/index.html> (infrastructure)

Core dependencies
-----------------

In order to compile and use Ojibwa language morphology and
dictionaries, you need:

- an FST compiler: [HFST](https://github.com/hfst/hfst), [Foma](https://github.com/mhulden/foma) or [Xerox Xfst](https://web.stanford.edu/~laurik/fsmbook/home.html)
- [VislCG3](https://visl.sdu.dk/svn/visl/tools/vislcg3/trunk) Constraint Grammar tools

To install VislCG3 and HFST, just copy/paste this into your Terminal on **Mac OS X**:

```
curl https://apertium.projectjj.com/osx/install-nightly.sh | sudo bash
```

or terminal on **Ubuntu, Debian or Windows Subsystem for Linux**:

```
wget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash
sudo apt-get install cg3 hfst
```

or terminal on **RedHat, Fedora, CentOS or Windows Subsystem for Linux**:

```
wget https://apertium.projectjj.com/rpm/install-nightly.sh -O - | sudo bash
sudo dnf install cg3 hfst
```

Alternatively, the Apertium wiki has good instructions on how to [install the dependencies for Mac
OS X](https://wiki.apertium.org/wiki/Apertium_on_Mac_OS_X) and how to [install
the dependencies on
linux](https://wiki.apertium.org/wiki/Installation_of_grammar_libraries)

Further details and dependencies are described on the GiellaLT [Getting Started](https://giellalt.uit.no/infra/GettingStarted.html) pages.

Downloading
-----------

Using Git:
```
git clone https://github.com/giellalt/lang-oji
```

Using Subversion:
```
svn checkout https://github.com/giellalt/lang-oji.git/trunk lang-oji
```

Building and installation
-------------------------

[INSTALL](https://github.com/giellalt/lang-oji/blob/main/INSTALL)
describes the GNU build system in detail, but for most users it is the usual:

```sh
./autogen.sh # This will automatically clone or check out other GiellaLT dependencies
./configure
make
(as root) make install
```
