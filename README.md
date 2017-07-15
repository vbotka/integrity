integrity
=========
[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)

*integrity* is a simple script to configure, maintain and verify atributes and hashes of selected files. It uses [hashdeep](http://md5deep.sourceforge.net/) and [mtree](https://www.freebsd.org/cgi/man.cgi?mtree(8)). Intended use is to schedule *integrity* from cron and email modifications if any were found.

**Tested** with FreeBSD and Ubuntu. Installation and configuration tested with [galaxy.ansible.com/vbotka/integrity](https://galaxy.ansible.com/vbotka/integrity/)

**Performance.** Checking integrity of the set (bin, lib, sbin, usr-bin, usr-lib, usr-lib32, usr-local-bin, usr-local-etc, usr-local-lib, usr-local-sbin, usr-sbin) of default FreeBSD system
- at standard cloud VM takes ~10s.
- at dedicated Intel(R) Pentium(R) CPU G3240 @ 3.10GHz takes ~3s.
