# Amazon blockers

Yeah so Amazon decided to be super shit and force-feed some of their tools upon people.

## Rufus

Rufus is an "AI" cursed horror that poses as a CS rep. If I wanted to be bothered by an entity, clanker or meat-based, while I shop, I'd go to physical locations. THE WHOLE POINT OF ONLINE SHOPPING IS TO NOT BE BOTHERED.

I found a base block on the [hollymathnerd substack](https://hollymathnerd.substack.com/p/how-to-kill-rufus), but it didn't work from the jump as of December 31st, 2025.

This form is what worked; it's a minor adjustment. This works as a user-provided custom filter in Brave Shield, and I'm assuming it would work the same in UBlock Origin.

```
amazon.com##.copilot-modal-container
amazon.com##div[data-copilot-name]
||amazon.com/*copilot*^$script
||images-na.ssl-images-amazon.com/images/*copilot*^$script
||m.media-amazon.com/images/*copilot*^$script
amazon.com##aside[data-copilot-chat-root]
amazon.com##div.copilot-chat-root
amazon.com##.left-nav-container
amazon.com##div[style*="left: 0px"][style*="position"]
amazon.com##.rufus-asin-faceout-header-left
amazon.com##[class^=”rufus-”]
amazon.com##div.rufus-chat-container
amazon.com##div.rufus-panel-container
amazon.com##body.rufus-docked-left:style(padding-left:0 !important; margin-left:0 !important;)
```