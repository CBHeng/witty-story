<div align="right">

[中文](daemon.md) | **English**

</div>

# `daemon` — guardian spirit

## What it does

A process that lives in the background with no controlling terminal, attached to nobody's login
session. Nobody calls it; it is simply awake — carrying mail, running schedules, listening on a
port. By convention the name ends in `d`: `sshd`, `httpd`, `crond`.

## Why it exists

Around 1963, MIT's Project MAC was running a time-sharing system on an IBM 7094. One machine
waited on many people at once — but some of the work belonged to nobody. Backups, schedules,
housekeeping. No one sat at a terminal waiting for them, and they had no business occupying
anyone's session. So that work got a process of its own: owned by no user, simply awake.

## Why the name

In 1867, Maxwell wrote to Tait that he wanted to pick a hole in the second law of thermodynamics.
Conceive, he said, "a finite being" who reads every molecule's speed at a glance and can do no
work at all except slide a massless shutter over a hole in a partition: it lets the slow ones
drift one way and the fast ones the other, so the hot side grows hotter and the cold side colder,
and "no work has been done, only the intelligence of a very observant and neat-fingered being has
been employed."

He did not name it. That was Kelvin, writing in *Nature* in 1874 about an army of "Maxwell's
'intelligent demons'" — with a footnote explaining the word "according to the use of this word by
Maxwell," who had never chosen it. Maxwell's own note reads: "Concerning Demons. 1. Who gave
them this name? Thomson." He tried to take it back: call him no more a demon but a valve, he
wrote. Nobody listened.

Nearly a century later Corbató, a physicist by training, [recognized the
creature](https://www.takeourword.com/TOW146/page4.html) — tireless, working in the background —
and handed its name to the processes doing the chores. Unix kept the older spelling: daemon, the
Greek daimōn, a lesser being that attends rather than torments.

## Credit

Fernando J. Corbató (1926–2019), who led CTSS and Multics and took the 1990 Turing Award for
them. The word came out of his group.

---

← [Back to the index](../README.en.md)
