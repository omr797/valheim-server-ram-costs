# Cheap Valheim Server: How Much RAM 2–10 Players Need, What Renewals Really Cost, and the Crossplay Details That Break Setups

A cheap Valheim server costs roughly **$6–8 per month at 4 GB of RAM** and **$12–16 per month at 8 GB**, billed monthly, based on what established hosts are showing on their Valheim pages. If your group is two to five people starting a fresh vanilla world, the 4 GB tier is enough. Buying more before you have built anything is the most common way a first server gets overspent.

Two things decide whether the cheap option stays cheap and actually works. The renewal price decides the first. Memory decides the second, and memory follows how much of the map you have explored and how much you have built, not how many people log in at the same time.

What follows: the current low-end price table, how to size RAM without guessing, the 10-player ceiling that makes "unlimited slots" a meaningless selling point, the save and crossplay details that decide whether your first week goes smoothly, the refund windows that differ by a factor of three, and when a bare-metal box from Spin Servers is the better buy than a managed game slot.

> **Quick answer**
> - 2–5 players, new vanilla world: 4 GB, about $6–8/month.
> - 6–10 players, or a world you have played for months: 6–8 GB, about $9–16/month.
> - Heavy mod pack plus large bases at 10 players: 10 GB and up.
> - Several game servers on one machine, or you want root access: a dedicated box, from $79/month at Spin Servers. 👉 [See Spin Servers' current dedicated server listings](https://bit.ly/Spinservers)

## What a cheap Valheim server costs right now

Prices are monthly, in the currency each host quotes, and come from the hosts' own Valheim pages. They change, so confirm at checkout.

| Host | 4 GB | 6 GB | 8 GB |
| --- | --- | --- | --- |
| Sparked Host | $6.00 | $9.00 | $12.00 |
| Gravel Host | $7.00 | $15.99 | $24.99 |
| Kinetic Hosting | not listed | $8.99 | not listed (12 GB is $15.99) |
| Gamehost | €7.99 | €10.99 | €13.99 |

At 8 GB the spread runs from $12.00 to $24.99 for the same amount of memory, so RAM stops being the thing you compare once you have picked a size. Kinetic Hosting's 6 GB plan includes 6 CPU threads and 5 backup slots; Sparked Host's 8 GB plan lists 3.5 vCPU and 100 GB of storage. Those are the differences that show up in-game, not the RAM number.

Treat "unlimited" as a question rather than a feature. In a recent r/valheim thread, a host advertised unlimited RAM and player slots, and the first reply asked what the guaranteed minimum was. That is the right question to ask any host before paying.

## How much RAM does a Valheim server actually need?

Memory tracks your save file. A map that has been explored for a hundred hours with three longhouses on it needs more RAM than a brand-new world with ten people standing in a meadow. Published guidance from hosts that support Valheim lines up with what long-running server owners report:

| Situation | RAM |
| --- | --- |
| Vanilla world, 2–5 players, new map | 4 GB |
| Vanilla world, 5–10 players, many hours in | 6 GB |
| Mod pack that adds content, up to 10 players | 8 GB |
| Large mod pack plus big bases, 10 players | 10 GB |

A regular on r/valheim put it the same way: memory use follows how much you have built and explored, not how many people are online, and for 8–10 players with crossplay they would want 8 GB and four real cores. Two independent sources landing on the same answer is about as much certainty as you get before you buy.

Crossplay does not change the memory math. It changes how players connect, which is a networking question, not a RAM one.

The one case where people routinely under-buy: importing an old world. A 200-hour save with a fortified base does not behave like a fresh map on the same plan. If you are moving a world over, size for what is already built.

## The 10-player ceiling

Valheim's dedicated server supports up to 10 players, and that limit comes from the game, not the host. A host that advertises "unlimited player slots" or "no player caps" is telling you something true about its billing and irrelevant to Valheim. Gravel Host and Kinetic Hosting both make that claim, and on a Valheim server it will never come into play.

Two practical consequences. First, a plan's player count tells you nothing when you compare Valheim hosts; compare CPU, backups, storage and mod tooling instead. Second, if your group is 12, you need two worlds on two servers, and that is a budget decision rather than an upgrade decision.

## The renewal price is the price you will pay

Intro discounts are where cheap Valheim hosting gets expensive. Gamehost's 8 GB plan shows **€11.19 for the first invoice and €13.99 after that**; the 4 GB plan shows €6.39 and then €7.99. The discount is 20% and it applies to one invoice, which is a month on monthly billing.

Some hosts run first-month promotions instead, where a plan advertised around $6 is a half-price first month and doubles afterwards. Both models are legitimate. The mistake is budgeting the intro number.

Compare at the renewal rate, and check two things on the checkout page: whether the discount applies to the first invoice or the first month, and what happens if you prepay annually. A 20% first-invoice discount on a yearly prepay is worth a lot more than the same discount on a monthly one.

## Setup details that decide whether a cheap server works

The hardware on a $6 plan is fine. Most first-server failures come from four settings.

**Password.** Valheim requires one for a dedicated server, at least five characters, and it cannot be the same as the server name. The panel enforces this, so set it before you invite anyone.

**Server name.** Skip accented characters like ä, é or č. With crossplay turned off, Steam can refuse connections to a name it cannot handle, and the error message will not tell you why.

**Crossplay.** Turn it on in the startup parameters. Steam players join the usual way; Xbox and Game Pass players join with the join code the server prints in the console at boot. With crossplay off, everyone connects using the IP and port shown in the panel. If your group is mixed PC and console, a host whose panel does not expose startup parameters is a hard no, because crossplay and world modifiers both live there.

**Saves.** The world autosaves every 30 minutes, and stopping the server from the panel forces a save immediately. Valheim ignores a `save` command typed into the server console. If you want a save on demand, add your character ID to `adminlist.txt` and type `save` in the in-game F5 console.

Moving hosts later is easier than most people expect. Upload the `.db` and `.fwl` world files through the file manager or FTP, restart, and the world is there. Characters are stored on each player's own machine, so nobody loses progress in the transfer.

Mods run on BepInEx, which you enable in the startup parameters. Plugins go into `BepInEx/plugins`, their settings into `BepInEx/config`, and every player needs matching versions or they will not connect. Many mod packs also need the Jotunn library. World modifiers such as combat difficulty, death penalty and resource rate are set in the startup parameters, with no file editing.

## Refund windows: 48 hours, 72 hours, or 7 days

- **Sparked Host:** 48 hours, full refund on game hosting. VPS and dedicated servers are excluded.
- **Gravel Host:** 72 hours, new customers' first hosting purchase only, one refund per account for life, minus processing fees. Renewals, trials, add-ons and upgrades are excluded; an initial annual plan may be prorated within 7 days.
- **Kinetic Hosting:** 7 days, and it covers renewal payments as well as first ones. If the service itself is at fault, the window extends to 14 days.
- **Spin Servers:** no money-back terms published on its server listings. Ask sales before you order.

A 72-hour window that excludes renewals is a much thinner safety net than a 7-day window that covers them. If you are importing an existing world, take the longer window. Problems with a migrated save tend to show up after the first proper session, not during it.

## When a $79 bare-metal box beats a $12 game slot

Spin Servers does not sell managed Valheim slots. It rents dedicated servers: root access, your own OS, no game panel, and nobody to fix your BepInEx install. The entry machine is a 4-core Xeon with 32 GB of RAM and 1 TB of NVMe for $79 a month.

| Server | CPU | RAM | Storage | Price/month | Order |
| --- | --- | --- | --- | --- | --- |
| Intel Xeon E3-1280 v5 (Dallas) | 4 cores / 8 threads, 3.7 GHz turbo | 32 GB DDR4 ECC | 1 TB NVMe | $79.00 | [View this server](https://bit.ly/Spinservers) |
| Intel Xeon E3-1280 v5 (San Jose) | 4 cores / 8 threads, 3.7 GHz turbo | 32 GB DDR4 ECC | 1 TB NVMe | $79.00 | [View this server](https://bit.ly/Spinservers) |
| Dual Intel Xeon Gold 6148 (Dallas) | 40 cores / 80 threads | 256 GB DDR4 | 2 × 1.92 TB SSD | $235.00 | [View this server](https://bit.ly/Spinservers) |
| Dual Intel Xeon Platinum 8173M (Dallas) | 56 cores / 112 threads | 512 GB DDR4 | 4 × 1.92 TB SSD | $390.00 | [View this server](https://bit.ly/Spinservers) |

Every listing includes 30 TB of monthly bandwidth on a 10 Gbps port and one IPv4 address. The E3 machines are described as suited to web hosting, VPN and gaming.

Run the per-head math before you talk yourself into it. Ten players splitting $79 pay $7.90 each. The same ten players on a $12–16 managed 8 GB slot pay $1.20–1.60 each. For a single Valheim world, the dedicated box is the expensive choice.

It wins in three situations. You want several game servers on one machine and the RAM to run them side by side. You want the save files on hardware you administer, with your own backup routine rather than a panel's. You are running a modded setup you want to control at OS level, where a panel's startup parameters are not enough.

What you take on is real work: installing the Valheim dedicated server with SteamCMD, applying updates, restarting after a crash, configuring the firewall, and setting up backups you have actually tested. If systemd and ufw are words you would have to look up, the $12 managed slot is cheaper once an evening of setup is priced in.

One more check before you commit: both locations are in the United States. Crossplay lets Xbox players join, but it does not fix physics lag, and an EU group on a Dallas box will feel it.

👉 [Check the current Spin Servers dedicated server lineup and prices](https://bit.ly/Spinservers)

## Pick by group size, then check three things

- **2–5 players, new vanilla world:** 4 GB. This is the cheapest tier at every host in the table and it is enough.
- **6–10 players, or a long-running world with big builds:** 6–8 GB.
- **Large mod pack plus large bases at 10 players:** 10 GB or more.
- **Several game servers, or you want root access:** a dedicated box.
- **More than 10 players:** two servers, because the ceiling is in the game.

Before you pay, confirm the renewal price and billing term, the refund window and what it excludes, and the server location relative to where your players actually live. Those three items account for most of the difference between a cheap Valheim server and an expensive mistake.

👉 [See Spin Servers' current dedicated server pricing](https://bit.ly/Spinservers)
