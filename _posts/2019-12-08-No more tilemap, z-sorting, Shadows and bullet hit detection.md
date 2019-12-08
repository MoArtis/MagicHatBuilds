---
layout: build
title: No more tilemap, z-sorting, Shadows and bullet hit detection
build_path: MH_191208
build_webgl_name: MH_WebGL
build_width: 960
build_height: 540
summary: "Using 3 kinds of renderer (Sprite, Tile and Mesh) was making the z-sorting
    nightmarish so I finally decided to just drop the tile-based floor in favor or
    using big plain sprites.<br>It\u2019s simpler to produce/handle and it might
    even look better on the long run (if constrained well-enough like in Isaac).\r
    Good thing, I can keep the somewhat efficient tile-based composite collider for
    static stuff like the pits/holes and the unbreakable walls.\nRelated to that
    switch, I implemented all the z-sorting functions for the Entities, the bullets
    and the walls (which are now just sprite but might end up being entities as well,
    like the spikes).<br>Shadows are in too. Since their implementation had close
    ties with z-sorting (which take into account the height of shadow casting things).
    It\u2019s completely fake using another procedural mesh for the bullets and an
    additional sprite renderer for the entities. I wanted no multiplicative / additive
    shadow so I went for a stencil-based shader. Maybe I\u2019m missing a much more
    obvious and flexible solution (Stencil = no AA) but that will do for now.<br>Finally,
    I got the bullet hit detection against entities integrated. The first step to
    rebuild the gamejam\u2019s version gameplay\u2026 after 2 weeks of work. :joy:<br>But
    at least, the build already allows to test the controls by trying to avoiding
    the bullet as long as possible. The player character has 4 HP and can \u201Cresurrect\u201D
    by pressing R.\r"
changelog:
  - Remove the Tile-based floor
  - Add proper Z-sorting for everything
  - Add stencil based shadows
  - Add simple Bullet to entity hit detection
downloads:
 - url: 
   title: PC Build
 - url: 
   title: Mac Build
 - url: 
   title: Linux Build
---
