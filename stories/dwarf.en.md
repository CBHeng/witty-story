<div align="right">

[繁體中文](dwarf.md) | **English**

</div>

# `dwarf`

## What it does

A system that pulls in financial data: it digs raw data out of its sources, cleans it,
transforms it, and refines it into numbers you can actually use.

## Why the name

In World of Warcraft, the dwarves are the ones who mine. The original opening cinematic puts
it plainly: "The stoic dwarves of Ironforge spent countless generations mining treasures from
deep within the earth."

Go back further and their ancestors, the earthen, were shaped by the titans out of [living
stone](https://warcraft.wiki.gg/wiki/Earthen), made for the express purpose of carving out the
deep places of the world.

And what a dwarf digs up isn't gold. It's ore. In the game, whatever you mine has to be hauled
to a forge and smelted into bars before it's worth anything.

Financial data is the same: what comes back is raw ore — rich, but useless until it's been
cleaned and refined.

Mining, smelting, storing — that's ETL in data engineering. The dwarf is the E.

## When I took it over

dwarf is a system I inherited, kept running, and went on to build out. Its methods were
crude. No elegant architecture, just one shovelful after another.

But it was steady, it was direct, and like any dwarf it stubbornly kept bringing the ore home.

The errors I ran into most weren't its own. A source page would have something wrong, or get
corrected after the fact, and the vein would shift, and the dwarf had to shift with it.

Dwarves aren't clever. It never noticed on its own; every time, someone had to show it where
to swing the pick.

Every time I changed it, it wasn't because it had broken. It was because the mountain had
moved.

## Credit

Whoever wrote `dwarf` is lost to history. All I know is that it was an old comrade-in-arms of
Peter Chen (who named [`tcell`](tcell.en.md)) — and a very good software engineer.

---

← [Back to the index](../README.en.md)
