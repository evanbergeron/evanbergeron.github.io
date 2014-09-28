---
layout: post
title: Some Useful Key Remappings
---

Caps-Lock -> Escape and Shift keys when tapped -> left and right parens.

Both of these were inspired by Steve Losh's infamous [A Modern Space Cadet](http://stevelosh.com/blog/2012/10/a-modern-space-cadet/) article. Months ago I followed the instructions to remap my caps-lock key and shift keys as instructed. I lived happily for many months.

But then I switched to linux and was unable to find similar instructions for linux. I found a couple lone souls out there trying to remap keys using xmodmap. But xmodmap (as far as I can tell) can't tell how long you hold down the keys for. I found a couple of hacks, but nothing worked for me.

Enter [xcape](https://github.com/alols/xcape). I cloned from github and entered

```./xcape -e 'Shift_L=Shift_L|parenleft'

./xcape -e 'Shift_R=Shift_R|parenright'

./xcape -e 'Caps_Lock=Escape'```

And viola. My main complaint about switching to linux was rectified. Hopefully this helps someone else out there as well :).


\- Evan
