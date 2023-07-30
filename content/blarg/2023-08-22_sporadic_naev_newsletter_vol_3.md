---
title: 'Sporadic Naev Newsletter Vol. 3'
author: bobbens
tags: [ 'development' ]
---

Rather than waiting 10 years again from the previous edition of our [sporadic
naev
newsletter](<%=@items['/blarg/2021-08-22_sporadic_naev_newsletter_vol_2.md'].path%>),
we've only let 2 years pass this time. In this edition, we'll talk about some
improvements in 0.10.0 that may have gone under the radar, and the upcoming
0.11.0 release.

#### State of 0.11.0

With a ton of commits and content since 0.10.0, things are starting to shape up
for 0.11.0. This release has focused greatly on reworking and improving
existing systems by bringing up to modern standards.

#### Universe Revisited

As [mentioned before on the
blarg](<%=@items['/blarg/2023-02-12_universe_revisited.md'].path%>), the
universe has been completely rework for 0.11.0. The universe should have a much
more natural feel that matches the lore, with the Sol Nebula being more
omnipresent as you travel around. This has required significant changes to many
systems and system objects, so that many places you knew will probably seem
familiar but quite different at the same time. It may take a while to get used
to.

TODO image

In numbers, some 67 new systems and 123 new space objects have been added,
mainly around the Sol Nebula to give a more in-depth sensation of destruction
and the fragility of humankind. Besides the typical planets and stations, these
systems also contain many secrets that you can uncover.

#### House Sirius Rework

For 0.10.0, the Soromid got a major rework by getting true bioships that can
level up and learn different skills, now it's only fair for the neglected House
Sirius to also get the same treatment. Instead of extreme biological
engineering, House Sirius relies on psychic abilities called flow. While
individuals don't possess very strong powers by themselves, House Sirius
has designed their ships to be powerful amplifiers to be able to unleash potent
abilities on the battle field.

TODO image of some ability

The player will also be able to obtain similar psychic powers and unlock the
full potential through new trials that can be found throughout space. Each
trial will require the player to overcome obstacles in order to unlock new
abilities and also increase their overall psychic powers.

TODO image of trial

While Sirius ships have flow capability built-in, other ships can also use
structural outfits to enable flow capability, allowing for more customization.
That said, Sirius ships get unique bonuses from flow powers which are not
available to other ships.

#### Plugin System

Although the [plugin system was introduced in
0.10.0](<%=@items['/blarg/2022-12-23_0.10.0.md'].path%>), it has gone largely
unnoticed. Currently, it is possible to replace and modify all parts of the
Naev that are implemented in Lua, which includes important parts such as
[autonav](<%=@items['/blarg/2023-07-30_new_autonav.md'].path%>), [many
outfits](<%=@items['/blarg/2021-06-06_lua_outfits.md'].path%>), [ship
explosions](<%=@items['/blarg/2023-07-18_ships_go_boom.md'].path%>), and more!
Not only that, Naev has option networking built in with
[enet](http://enet.bespin.org/), allowing for networking functionality. On this
line, there is a very much WIP [multiplayer
plugin](https://github.com/ThrosturX/naev-multiplayer), that allows for playing
with other people. To make development somewhat easier, a [development
manual](https://naev.org/devmanual/) is being worked on, which covers things
like how to write content for Naev and how to structure plugins. Given the
advanced programming possibilities with the [Naev Lua
API](https://naev.org/api/), the only limit is your imagination!

TODO image of plugins menu

Oh, there is [explicit support for total
conversions](https://github.com/naev/total_conversion_plugin_example) too!

#### New Content

PD
Minerva
New NPC
New accessories
Space Trader Society

#### Game Optimization

One issue Naev has traditionally had with the large systems it features, is
slow downs when many pilots were fighting each other as a result of a primitive
collision system. Well, it is no longer an issue as the current system has been
reworked with quadtrees. Testing shows that it is much much faster in extreme
cases, with the game easily handling hundreds of ships fighting each other
without slowing down. Furthermore, many aspects of the game have been profiled
and optimized such that the game should run much more fluid than 0.10.0.

TODO image pushing FPS limits

#### Concluding Remarks

This concludes the Sporadic Naev Newsletter Vol. 3, and see you again in
the next one!