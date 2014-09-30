---
layout: post
title: Fonts, Icons and some Magick!
excerpt: "<p>First, <a href=http://www.imagemagick.org/script/binary-releases.php>Install ImageMagick</a> - a great tool for manipulating images and videos. After that, we can turn text and symbols into images. 
<p>I know, I know, it's not that fancy. If your Photoshop skills are up to snuff, this tutorial will seem like baby games. But as an iOS developer with no Photoshop experience, I needed a way to make simple icons: play buttons, gears, and other things that I took for granted when I had a full-time designer on my team."
---

First, [Install ImageMagick](http://www.imagemagick.org/script/binary-releases.php) - a great tool for manipulating images and videos. After that, we can turn this 

```convert -background none -fill blue -gravity center
 -pointsize 36 -font /System/Library/Fonts/AppleSDGothicNeo-Bold.otf 
 caption:"Install ImageMagick\!"```

into this

![ImageMagick formatted and colorized output text]({{ site.baseurl }}/images/imagemagick.png)

I know, I know, it's not that fancy. If your Photoshop skills are up to snuff, this tutorial will seem like baby games. But as an iOS developer with no Photoshop experience, I needed a way to make simple icons: play buttons, gears, and other things that I took for granted when I had a full-time designer on my team. 

Enter Apple Fonts. With glyphs for almost every part of the Apple system, we've got a treasure trove on our hands.
![Apple System Font glyphs]({{ site.baseurl }}/images/applesystemfont.jpg)

Using the code in the earlier example, we can swap out `Apple Symbols.tff` for `AppleSDGothicNeo-Bold.otf` and use the text representation of the glyph we want (say, the caduceus -- you know, the winged staff on the side of US ambulances) like so 

        convert -background none -fill blue -gravity center 
   -pointsize 36 -font /System/Library/Fonts/Apple\ Symbols.tff 
   caption:"☤"

to get ![Caduceus image from the Symbols Font]({{ site.baseurl }}/images/caduceus.png)

The hardest part is finding the text for the symbol! Then you can import these PNG icons into your latest project and look like a professional designer.
