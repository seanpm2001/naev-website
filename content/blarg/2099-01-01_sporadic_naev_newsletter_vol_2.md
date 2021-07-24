---
title: Sporadic Naev Newsletter Vol. 2
author: bobbens
tags: [ 'development' ]
---

So it's been over 10 years from the first edition of our [sporadic naev
newsletter](<%=@items['/blarg/2010-07-16_sporadic_naev_newsletter_vol_1.md'].path%>),
so it seems like it might be a good time to have the second edition. In the
previous edition, we talked about the state of 0.5.0 and the introduction of
big systems and electronic warfare. In this edition, we'll talk about the state
of 0.9.0 and new features like stealth and safe lanes.

#### State of 0.9.0

We've passed 4,700 commits from 0.8.2. This is going to be the largest amount of
content and changes from any release ever with tons of graphical improvements,
new mechanics, and new content added all over. It is already all live in the
nightly images which are available from both
[github](https://github.com/naev/naev/releases/tag/nightly) and steam via the
opt-in beta. That said, it is recommended for you to back up your save or use a
new one if you attempt to do this. At the current moment, you will lose many
outfits and experience hiccups trying to use an old save game. Unlike the
official releases, the nightly is still rather unpolished.

Currently there is no hard ETA for the release, but we hope to release it
within the year and follow a more timely release cycle. We hope that we'll be
able to do a feature freeze in a couple of months and focus exclusively on
polish until the release. As always, we will release one or more betas before
the official release to try to debug potential issues.

#### Electronic Warfare Overhaul

Electronic warfare was originally introduced in 0.5.0. With the move to big
systems, it no longer made sense for all ships to be visible at all times.
Furthermore, we wanted to differentiate the roles between smaller and larger
ships, while aiding survivability of small ships by making it harder for the
largest of turrets to track them and hit them. While this worked well to some
extent, it was never transparent to the player. We've revamped it this time
around to be fully visible to the player. Each ship, depending on its mass and
bonuses, will have three separate values: detection, evasion, and stealth, that
control when the ship is first detected, when the ship details are shown and
scanning is possible, and finally how well the ship can stealth.

SHOW EXAMPLE

Hiding is the most important attribute that controls when ships are detected at
and affects both evasion and stealth. Evasion is usually 75% of detected at
value, and controls how well turrets and missiles track a ship. Furthermore, it
controls the distance at which a ship is scanned at. Scanning a ship allows you
to see the details of cargo and outfits. Furthermore, patrol ships will scan
your ship and make sure you don't have illegal cargo.

SCANNING EXAMPLE

That leads us to the final mechanic: stealth! Stealth allows ships to become
completely invisible if no ships are within their stealth distance. When
stealthed, ships get a -50% penalty to all movement: max speed, thrust, and
turning. However, they cease to appear on all system sensors. This allows ships
to sneak past systems or ships, opening lots of opportunities for contraband,
piracy, and survival.

STEALTH EXAMPLE

#### Safe lanes

safe lanes

#### Rebalance

Lots of shit

#### Ship Classification Redux

This is a more minor change, but rare ship classes, such as cruiser ships, or
motherships have been removed. Other similar classes have been merged, such as
heavy drones and fighters, which retain the name of fighters. Furthermore,
fighters have been split into fighters and interceptors (light fighters), and
cruisers have been split into cruisers and battleships (heavy cruisers). This
changes are mainly there for the equipment algorithm and AI to exploit.

#### Visual Novel Framework


#### Future Steps

There are lots of other improvements we have not mentioned in this newsletter:
linear programming-based equipment optimization, discoveries, new missions, new
ship attributes, more shader support, etc. We might go deeper into new features
in future blarg posts as we refine and polish the mechanics.

With regard to what is coming up, there are no too major things left to do.
Besides overall polish, which will take most of the time, some new missions
have to be written, in-system objects implemented, jamming rework, pricing
rebalance, and a few odd ends here and there. We're hoping for a release within
this year, but given the ambition and scope of 0.9.0, we'd rather delay and
have a better release, than rush it and have it be unplayable.

If you wish to contribute to Naev, we have lots of things that can be done,
even without programming experience! From [making cooler beauty shops for comm
and shipyard window](https://github.com/naev/naev/issues/1835), [adding an
uninhabited frontier](https://github.com/naev/naev/issues/1866), [more loading
screens](https://github.com/naev/naev/issues/1814), [new character
artwork](https://github.com/naev/naev/wiki/Needed-Artwork%3A-Characters), [new
outfit artwork](https://github.com/naev/naev/wiki/Needed-Artwork%3A-Outfits),
[more missions](https://github.com/naev/naev/wiki/Mission-Scripting), gameplay
testing, etc.  Tasks to be done can be found on the [issue
tracke](https://github.com/naev/naev/issues), and discussion can be had on
[Discord](https://discord.com/invite/nd2M5BR).

This concludes the Sporadic Naev Newsletter Vol. 2, and hopefully the next will
be sooner than 10 years from now.

