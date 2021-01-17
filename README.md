# Ever wondered how to use Apache Creadur RAT? Here's creadur-rat-examples

Since living code is easier than documentation this project is supposed to contain some
examples on how to configure Creadur RAT from ASF.

[https://creadur.apache.org/rat/](RAT project page)
[https://creadur.apache.org/rat/apache-rat-plugin/check-mojo.html](Maven Mojo definition)

In case of errors feel free to contact <a href="&#109;&#97;&#105;&#108;&#116;&#111;&#58;&#112;&#111;&#116;&#116;&#108;&#105;&#110;&#103;&#101;&#114;&#64;&#97;&#112;&#97;&#99;&#104;&#101;&#46;&#111;&#114;&#103;&#63;&#115;&#117;&#98;&#106;&#101;&#99;&#116;&#61;&#82;&#65;&#84; &#101;&#120;&#97;&#109;&#112;&#108;&#101;&#115; &#97;&#116; &#71;&#105;&#116;&#104;&#117;&#98;">me</a> or start a pull request :-)

## Travis integration

In order to run all examples a main pom.xml is provided that is taken into account from Travis.

[![Build Status](https://travis-ci.org/ottlinger/creadur-rat-examples.svg)](https://travis-ci.org/ottlinger/creadur-rat-examples)

## Codacy

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/00f1aaecada54cf09c9b505e410a0a11)](https://www.codacy.com/gh/ottlinger/creadur-rat-examples/dashboard)

## Examples that work with newer SNAPSHOT versions only

In some cases features only work with the current SNAPSHOT version and are disabled here:

* RAT-262: requires a recent 0.14-SNAPSHOT with ignoring JSON-capabilities
