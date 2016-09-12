integrity
=========
[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)

integrity is a simple script to verify files' atributes and hashes. Uses [hashdeep](http://md5deep.sourceforge.net/) and [mtree](https://www.freebsd.org/cgi/man.cgi?mtree(8)). Intended use is to schedule it in cron and email admin the changes.

**Tested** with FreeBSD and Ubuntu. Installation and configuration tested with https://galaxy.ansible.com/vbotka/ansible-integrity/

**Performance.** Checking integrity of the set (bin, lib, sbin, usr-bin, usr-lib, usr-lib32, usr-local-bin, usr-local-etc, usr-local-lib, usr-local-sbin, usr-sbin) of default FreeBSD system

- at a standard cloud VM takes ~10s.
- at dedicated Intel(R) Pentium(R) CPU G3240 @ 3.10GHz takes ~3s.
