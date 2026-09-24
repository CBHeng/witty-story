<div align="right">

[中文](tcell.md) | **English**

</div>

# `tcell` — T-cell

## What it does

A monitoring service that patrols every service on a host, finds the ones that have hung and
stopped answering, and kills the process. Getting back up is somebody else's job.

## Why it exists

Services would hang; servers would fall over. The hangs were usually a deadlock, and tracking
one of those down takes a long stretch of time — time a small team doesn't have, and not while
the product's SLA is on the line. In a distributed system these failures are random and
occasional: you never know when the next one is due.

The CTO's call was to defend the SLA first. tcell came together quickly: watch the services on
a single host, kill the ones that have gone bad. Killing is all it does, because every service
already had a start script attached — tcell kills, the service comes back on its own. Random
failure got held to a level we could live with, and it bought the thing we actually needed:
time to go after the deadlock at the root.

## Why the name

T-cells are the immune system's patrol. They don't repair a broken cell — they roam
the body, recognize the ones that have gone bad, and destroy them, leaving the body
to grow the tissue back. A standing mercenary force for the body's own upkeep.

## Credit

The name `tcell` came from Peter Chen, our CTO at the time — a software architect with real
depth and a craftsman's temperament, and someone who knew how to make the call when resources
were thin and the fire was already burning. tcell is what that call left behind, and the
system that has stayed with me ever since.

---

← [Back to the index](../README.en.md)
