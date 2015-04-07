---
layout: post
title: XCode Color Palettes 
---

I was working on a project recently with a group at work and it occurred to me that we had no way to share colors in IB. Either each developer had to punch in the RGB values every time, or you just had to wing it.

Enter Color Palettes. 

![color palette](/images/colorpalette.png) 

By saving a set of colors as a color palette, you can easily ship the backing file around between developers or even designers!

Simply copy the corresponding `.clr` file into your local `~/Library/Colors`, and restart XCode. The color palette should appear automatically.
<img src="/images/colorpalettedemo.gif" width="400" height="300" />

I've even seen information on how to [import a photoshop color swatch as an XCode color palette](http://blog.thefrontiergroup.com.au/2014/09/how-to-import-a-photoshop-colour-swatch-into-xcode-storyboards-os-x-colorpicker-palette/), so your design team can get in on the action.
