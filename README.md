# witty-story

> 那些富有故事性的軟體事跡：讓人印象深刻、恍然大悟，聰慧而有意義。偶爾帶點幽默 —— 開發者才懂的會心一笑，不是嘲笑，是一種滿足的驚喜。
>
> *Software stories worth telling: the ones that stay with you, that make something click,
> that turn out smarter and more meaningful than they first looked. Now and then one is
> funny, in the way only developers catch — never a laugh at anyone's expense, but the
> satisfying kind of surprise.*

---

## `tcell` — T 細胞 / T-cell

巡邏伺服器上的所有服務，偵測到卡死、沒有反應的，就把它的 process 殺掉。T 細胞也是這樣在體內巡邏的 —— 它不修理壞掉的細胞，它清除，然後交給身體自己長回來。

It patrols every service on a host and kills the process of any that has hung and stopped
answering. T-cells work the same beat: they don't repair a bad cell, they remove it and
leave the body to regrow the tissue.

> **殺死是一種治療。** ***Killing is a form of healing.***

→ [更多詳細 / Read more](stories/tcell.md)

## `daemon` — 守護行程 / guardian spirit

`sshd`、`httpd` 尾巴上的那個 `d`，是 daemon（守護靈）。而 daemon 來自 Maxwell 想像出來的那個小東西：守在隔板的孔邊，無休無止地分類分子，只為了證明熱力學第二定律「只有統計上的確定性」。這個拼法比 demon 更老 —— 希臘文裡，它指的是在旁照看你的那種存在。

The `d` on the end of `sshd` and `httpd` is for daemon, and the daemon is the creature Maxwell
imagined at a hole in a partition, sorting molecules without rest for no better reason than to
show that the second law of thermodynamics "has only a statistical certainty." The spelling is
older than demon: in Greek, a being that attends you.

> **它不是惡魔，是守著你的那個靈。** ***It was never a demon. It's the spirit that keeps watch.***

→ [更多詳細 / Read more](stories/daemon.md)

## [`cargo cult programming`](https://zh.wikipedia.org/zh-tw/%E8%B4%A7%E7%89%A9%E5%B4%87%E6%8B%9C%E7%BC%96%E7%A8%8B) — 貨物崇拜式編程 / cargo cult programming

那三行為什麼在那裡？「拿掉會壞」—— 而沒有人試過拿掉。你想起某些同事問過，也想起自己好像這樣答過。再往下想，那三行說不定就是自己留下的 —— 現在換成別人在問，答案沒變。Feynman：南太平洋那群人蓋好跑道、塔台，戴上木頭削的耳機，正在等著飛機。每一件事都做對了，但沒有飛機降落。

Why are those three lines there? "It breaks without them" — nobody tried. You remember
colleagues asking, and giving that answer yourself. Some may be lines you left behind — and
now somebody is asking. Same answer. Feynman: islanders who built a runway and a control
tower, wore two pieces of wood for headphones, and waited. Everything done right, and no
airplanes landing.

> **這不是寫錯，是照著對的樣子寫。** ***It isn't wrong code. It's code shaped like right code.***

→ [更多詳細 / Read more](stories/cargo-cult-programming.md)
