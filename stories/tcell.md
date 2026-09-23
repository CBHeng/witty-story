# `tcell` — T 細胞 / T-cell

## 它做什麼 / What it does

一種監控服務：巡邏伺服器上的所有服務，偵測到已經卡死、沒有反應的，就把它的 process 殺掉。怎麼重新起來，不是它的事。

A monitoring service that patrols every service on a host, finds the ones that have hung and
stopped answering, and kills the process. Getting back up is somebody else's job.

## 為什麼會有它 / Why it exists

服務會卡死，伺服器會過載。卡死的原因多半是 deadlock，但要將它排查出來得花上很長一段時間 —— 小團隊沒有那個資源，也沒辦法在排查期間對產品的 SLA 打包票。這類故障在分散式系統裡是隨機的、偶發的，我們不知道它什麼時候來。

當時 CTO 的決定是：先守住眼前的 SLA。於是很快做出了 tcell，監控單台伺服器上的服務，發現壞死的就殺掉。殺完不用管，因為每個服務都綁了自動啟動的腳本 —— tcell 只要負責殺，服務自己會重新起來。隨機性故障因此被壓在一個可以接受的水準上，而我們真正需要的東西也買到了：一段可以專注去追 deadlock 根因的時間。

Services would hang; servers would fall over. The hangs were usually a deadlock, and tracking
one of those down takes a long stretch of time — time a small team doesn't have, and not while
the product's SLA is on the line. In a distributed system these failures are random and
occasional: you never know when the next one is due.

The CTO's call was to defend the SLA first. tcell came together quickly: watch the services on
a single host, kill the ones that have gone bad. Killing is all it does, because every service
already had a start script attached — tcell kills, the service comes back on its own. Random
failure got held to a level we could live with, and it bought the thing we actually needed:
time to go after the deadlock at the root.

## 為什麼這樣取名 / Why the name

T 細胞是免疫系統派出去的巡邏兵。它不修理壞掉的細胞——它在體內巡邏，辨識出已經感染或失能的細胞，然後把它們清除，剩下的交給身體自己長回來。一支維護身體的監控傭兵。

T-cells are the immune system's patrol. They don't repair a broken cell — they roam
the body, recognize the ones that have gone bad, and destroy them, leaving the body
to grow the tissue back. A standing mercenary force for the body's own upkeep.

## 致敬 / Credit

`tcell` 這個名字出自當時的 CTO Peter Chen —— 一位技術深厚的軟體架構師，帶著工匠魂的職人心態，也懂得在資源有限、災難當前的時候做出取捨。tcell 就是那個取捨留下來的東西，也是讓我印象深刻的系統。

The name `tcell` came from Peter Chen, our CTO at the time — a software architect with real
depth and a craftsman's temperament, and someone who knew how to make the call when resources
were thin and the fire was already burning. tcell is what that call left behind, and the
system that has stayed with me ever since.

---

← [回索引 / Back to the index](../README.md)
