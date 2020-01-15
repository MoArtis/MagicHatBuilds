---
layout: build
title: Not sick anymore! Map structure, Enemy logic and anim, better bullet patterns
build_path: MH_200114
build_webgl_name: MH_WebGL
build_width: 960
build_height: 540
summary: "I was super sick and slow so was the progress. This build tests a new
    map structure, add a enemy behavior system and improves on some major features.\nThere
    is a new bullet pattern system as the old one was not flexible enough. It allowed
    nice looking patterns and will be useful for bosses and crazy situations. But
    it was too limited for enemies that should use patterns with very specific shapes
    and behaviors. Like most enemies in Enter the Gungeon or Monolith. \nAnimating
    and controlling the enemies is always a challenge for me in term of how to implement
    these \"states\" properly. I always try to make my own system but this time I
    want to try the unity way again using Mecamin. I went a step further by using
    a layer of the animator to manage the enemies \"logic\" using custom \"BehaviorScript\"
    extending the StateMachineBehaviour class. Seems to work fine and it should be
    flexible enough. We will see how it goes on the long term.\nThe Isometric view
    is much more painful to integrate properly than expected. Everything needs to
    be accounted for its skewed nature, it's a big pain in the ass. But at least
    it looks somewhat more unique than a \"flat\" view."
changelog:
  - Add new map structure
  - Add a flexible bullet pattern system (shapes!)
  - Add enemy animation system (It's just Mecanim)
  - Add enemy behavior system (using Mecanim!?)
  - Fix ton of issues related to the isometric view 
downloads:
 - url: 
   title: PC Build
 - url: 
   title: Mac Build
 - url: 
   title: Linux Build
---
