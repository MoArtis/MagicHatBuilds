---
layout: build
title: Spike, Hp/Dmg management and movement stuttering
build_path: MH_191128
build_webgl_name: MH_WebGL
build_width: 960
build_height: 540
summary: "I needed to test inter-entity interaction for my entity framework so I
    integrated some spikes.<br>If the character walks 4 times on them, it will lose its
    4 hp and die. Simple but it proves that this approach is efficient and extensible.<br>A
    big invisible change is the tilemap. I figured a way to generate it from code
    by reading custom level data. This will allow us to have proper level design tools.
    I'm also testing Chunk rendering mode in this build. Performance should be much
    better.<br>Movement and collision management is always a important topic. I lost
    a lot of time on my previous projects on that with complex custom logic to entirely
    avoid Unity's physics. Not this time, I want to get the most of Unity Collider
    and Rigidbody classes. It might be tricky to tweak and control but it seems to
    me the only to save a ton of time on this project. This build is testing a setup
    using dynamic rigidbodies using add force. By forcing the physic engine to update
    60 times per second, it seems to feel alright. It's probably not solid but we
    will work around the problems along the way. Since the fixed timestep value can
    be tweaked at runtime, we can adapt it to the player needs (when not using vSync
    or 144hz monitor...).<br>I finally I did some blender to make a bad card model for
    the proto enemy. :smile:"
changelog:
  - Add basic inter-entity interaction (spikes)
  - Add an health and damage system with stats
  - Test a better tilemap implementation
  - 'Improve the (proto) movement logic (no more stutter) '
  - Add a trashy test model for the card enemy
downloads:
 - url: 
   title: PC Build
 - url: 
   title: Mac Build
 - url: 
   title: Linux Build
---