---
layout: build
title: Invisible system work for visible gameplay integration!
build_path: MH_191220
build_webgl_name: MH_WebGL
build_width: 960
build_height: 540
summary: 'This build a many very basic but critical system. They are quite "invisible"
    for now but they will allow to create many variations of gameplay (item?). In
    this build, I used that Modifier system to manage the knockback and invulnerability
    on hit. It''s completely event driven so it should allow us to attach special
    effects on many different aspect of the game like an enemies who spawn bullets
    or other enemies on death.<br>I got stuck for too long on that topic. But
    after that I was able to advance ""quickly"" on the core gameplay. Namely the
    absorption, the absorbed bullet stocks (represented as card in the bottom left)
    and a way to fire them back at them with a chargeable shot.<br>The "weapon"
    and the absorb mechanic are already quite modular (that can be used for different
    "items" maybe) but as I haven''t integrated a way to tweak them at runtime, they
    can used in only one way in this build. Maybe later.'
changelog:
  - Fix bullet hit detection (non-iso box cast)
  - Add Event/modifier system
  - Add invulnerability on hit
  - Add Charging fire mechanic
  - Add bullet stock management
  - Add absorb mechanic
  - Add collectible entities (Healing collectible as an example)
  - Add art and effect for testing (basic feedbacks)
  - 'Add some UI elements (HP counter and bullet stocks) '
downloads:
 - url: 
   title: PC Build
 - url: 
   title: Mac Build
 - url: 
   title: Linux Build
---
