master: [![Build Status](https://travis-ci.org/x-stream/xstream.svg?branch=master)](https://travis-ci.org/x-stream/xstream) [![Coverage Status](https://coveralls.io/repos/github/x-stream/xstream/badge.svg?branch=master)](https://coveralls.io/github/x-stream/xstream?branch=master)  
v-1.4.x: [![Build Status](https://travis-ci.org/x-stream/xstream.svg?branch=v-1.4.x)](https://travis-ci.org/x-stream/xstream) [![Coverage Status](https://coveralls.io/repos/github/x-stream/xstream/badge.svg?branch=v-1.4.x)](https://coveralls.io/github/x-stream/xstream?branch=v-1.4.x)

- - - -
# XStream
_Java to XML Serialization, and back again_

## Binaries
All binary artifacts are bundled in the -bin archive.  It includes
the XStream jars and any other library used at build time, or
optional runtime extras.  MXParser is recommend for use as it will
greatly improve the performance of XStream.

## Documentation
Documentation can be found at [GitHub](http://x-stream.github.io).  This
includes:
* [Introduction](http://x-stream.github.io) and [Tutorials](http://x-stream.github.io/tutorial.html)
* [JavaDoc](http://x-stream.github.io/javadoc/index.html)
* [Change History](http://x-stream.github.io/changes.html)
* [Frequently Asked Questions](http://x-stream.github.io/faq.html)

## Source
The complete source for XStream is bundled in the -src archive.  This includes:
* Main API [xstream/src/java]
* Unit Tests [xstream/src/test]
* Maven Build Files [pom.xml]
* Hibernate Module [xstream-hibernate]
* Website [xstream-distribution]

## About this fork

This is trunk of the XStream repo at
https://github.com/x-stream/xstream as of 9/20/22. It includes the
patches from pull request https://github.com/x-stream/xstream/pull/299
which the original report
https://bugs.chromium.org/p/oss-fuzz/issues/detail?id=49858 says fixed
https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-40151 .

I've also made changes to DefaultDriver.java to switch the default XML
parser back to Xpp3, to make the change as minimal as possible.
