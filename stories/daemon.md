# `daemon` — 守護行程 / guardian spirit

## 它做什麼 / What it does

在背景常駐的行程：沒有控制終端，不掛在任何人的登入階段底下。沒有人呼叫它，它自己醒著 —— 收信、跑排程、聽著一個 port。名字習慣以 `d` 結尾：`sshd`、`httpd`、`crond`。

A process that lives in the background with no controlling terminal, attached to nobody's login
session. Nobody calls it; it is simply awake — carrying mail, running schedules, listening on a
port. By convention the name ends in `d`: `sshd`, `httpd`, `crond`.

## 為什麼會有它 / Why it exists

1963 年前後，MIT 的 Project MAC 在 IBM 7094 上跑分時系統。一台機器同時伺候很多人，但有些工作不屬於任何人：備份、排程、雜務。沒有人坐在終端機前等它們，也不該佔著誰的 session。於是它們有了自己的一種行程 —— 不歸任何使用者，自己醒著。

Around 1963, MIT's Project MAC was running a time-sharing system on an IBM 7094. One machine
waited on many people at once — but some of the work belonged to nobody. Backups, schedules,
housekeeping. No one sat at a terminal waiting for them, and they had no business occupying
anyone's session. So that work got a process of its own: owned by no user, simply awake.

## 為什麼這樣取名 / Why the name

1867 年，Maxwell 寫信給 Tait，說想在熱力學第二定律上「挑個洞」：設想一個「有限的存在」（a finite being），一眼看穿每顆分子的速度，除了拉動隔板上那片沒有質量的滑板以外做不了任何工。它只放慢的分子過去、快的回來，熱的更熱、冷的更冷 ——「沒有做任何功，用掉的只有一個眼尖手巧的存在的智慧」。

名字不是他取的。1874 年 Kelvin 在《Nature》上寫下「Maxwell 那支聰明的 demon 大軍」，註腳還說這是「Maxwell 對這個字的用法」—— 但這個名字從來不是 Maxwell 取的。他自己的筆記寫著：「關於 Demons。一、這名字誰取的？Thomson。」他甚至抗議：別再叫它 demon，叫它閥門吧。沒有人理他。

近一百年後，物理出身的 Corbató [認出了這個東西](https://www.takeourword.com/TOW146/page4.html)：無休無止，在背景工作。而 Unix 留下的是更老的拼法 daemon —— 希臘文的 daimōn，在旁照看，不分善惡。

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

## 致敬 / Credit

Fernando J. Corbató（1926–2019），CTSS 與 Multics 的主持人，1990 年圖靈獎得主。daemon 這個字，出自他帶的那個團隊。

Fernando J. Corbató (1926–2019), who led CTSS and Multics and took the 1990 Turing Award for
them. The word came out of his group.

---

← [回索引 / Back to the index](../README.md)
