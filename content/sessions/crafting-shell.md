---
key: crafting-shell
title: 'Learning Computer Systems by Crafting: Shell （作って学ぶシェル）'
id: crafting-shell
format: conference
talkType: ""
allroom: false
speakers:
- shibu_jp
---
We sometimes discuss newbies how to learn shell because it is like air. Let's learn shell and computer systems by crafcting a subset of the POSIX shell via Go.

---

There are few opportunities to learn shell explicitly. In these days, knowledge of the shell is more important to use modern technologies. For example, to create more portable/secure container images needs shell's features like environment variables and more.

* Shell 101
  * What is a shell?
  * Features required for CUI shell
* Shell's state
  * Environmental variables
  * PATH
  * Current Working directory
  * Exit code
  * Files (what are 0, 1, 2?)
* What is the difference between passing a process start argument as a string and passing it as an array in Docker?
  * Differences in whether or not to use shell, which is often seen in process startup APIs
* Unix Philosophy and 12 FACTOR APP
* Shell made and learned with Go
  * Go's os/exec behavior
  * Read the POSIX specifications