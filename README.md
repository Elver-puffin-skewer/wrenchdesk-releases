# WrenchDesk

Shop management for small engine repair — mowers, pressure washers, tillers, generators,
chainsaws, and whatever else rolls through the door.

It replaces the notebook: customers, their equipment, estimates, repair history, parts on order,
and what money actually came in today and this week. It runs entirely on the shop's own PC. No
subscription, no cloud account, no per-user fee.

**This is where you download it.** The program itself is built elsewhere; this page exists to hand
you the file.

---

## Install it

Go to [**Releases**](../../releases), download **`WrenchDesk.exe`**, and double-click it.

That is the whole install. One file, nothing else to download, nothing else to install — no .NET,
no runtime, no setup wizard. The first time you run it, it asks whether to set itself up. Press
Enter and it copies itself somewhere permanent, puts an icon on your desktop, adds itself to the
Start menu, and starts.

It installs under your own user account, so there is **no administrator prompt**.

> **Windows will warn you** that the publisher is unknown, because the file is not code-signed.
> Choose **More info** then **Run anyway**.

## Update it

Download the new `WrenchDesk.exe` and run it again. Your customers, tickets and payments live in
`Documents\WrenchDesk` and are never touched by an update.

When a new version needs to change how the records are stored, it **copies them first** — into
`Documents\WrenchDesk\Backups\before-upgrade-*.db` — before changing anything. If that copy cannot
be written, the update does not go ahead and nothing is altered.

## Remove it

```
WrenchDesk.exe --uninstall
```

Your shop data is left alone.

---

## What you see when it runs

Nothing, which is the point. WrenchDesk opens your browser and then sits **down by the clock**, in
the notification area. Closing the browser does not stop it — only *Stop WrenchDesk* on the tray
icon does.

Right-click the tray icon for the shop screen, the address to use from a phone or tablet, the
records folder, and the way to shut it down.

## From a phone or tablet

The second address shown works from any phone, tablet or laptop on the same wifi — handy for
writing up an estimate at the bench, or checking a delivery address without walking back to the
counter. The layout adapts to a small screen.

The first time you run it, Windows Firewall may ask whether to allow WrenchDesk on the network.
Say yes to **Private networks** for the tablet address to work.

> [!CAUTION]
> **Do not put the database on a network share** and open it from two PCs. Leave the file on the
> shop PC and reach it over the address above — then exactly one program ever touches it, which is
> the supported arrangement.

## Back it up

Everything the shop has is one file, plus a folder of photos. Under **Settings** you can back up to
a USB stick on demand, or set a daily or weekly schedule that writes to one or two places at once.
Scheduled backups are **off until you turn them on**.

---

## Help

A full guide lives inside the program under **Help**, written for the counter rather than for a
developer. It works offline and shows your shop's actual settings — where the records are, whether
backups are on, the exact address to type into a phone.

---

Copyright © 2026 Thomas Marks.
