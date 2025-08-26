# [McMMO](https://github.com/mcMMO-Dev/mcMMO) Bug Fix Report
## This is a repository to show that I helped fix a bug on an open-source software (Spigot Minecraft plugin) called [McMMO](https://github.com/mcMMO-Dev/mcMMO) back in 2016, by reporting an issue relating to efficiency 6+ being removed whenever smelting or anviling was done.

## What was the issue (Brief)?

The issue was whenever I played on any Java-based Minecraft server that used [McMMO](https://github.com/mcMMO-Dev/mcMMO) such as McOrigins, Purple Prison, or Minecraft Central back in around 2015-2018, whenever I tried to anvil or furnace pickaxes or axes with efficiency greater than 5, the result would give me a efficiency 5 of that same item in question. This was irritating to me and because I was dealing with local Minecraft server hosting myself at the time experimenting with free ones then paid ones later on along with a great interest in Spigot and Bukkit plugins, I tracked down the issue to [McMMO](https://github.com/mcMMO-Dev/mcMMO) by myself. After that, since I realized I did not know how to code at the time, I knew I could still report the issue anyway. So I did. I found out [McMMO](https://github.com/mcMMO-Dev/mcMMO)'s GitHub and reported the issue. Then on July 23, 2018, a fix was implemented by [t00thpick1](https://github.com/t00thpick1), and it was marked as completed on July 24, 2018. This shows that I have been caring about supporting open-source software ever since September 18, 2016, and that I have a great interest in supporting everyone, including myself, as much as I can!

## What was the issue (Long)?

For proof of everything, I have links and screenshots to support my claims.

[This](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/3033) is where the issue was reported by me for [McMMO](https://github.com/mcMMO-Dev/mcMMO).

This is a screenshot of that issue page:
<img width="1262" height="594" alt="image" src="https://github.com/user-attachments/assets/e97f1331-5419-4b0c-a739-c3b7f33ce43b" />

### Where is the commit that solved the issue?

[This](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/commit/fbe26af2d7dbb841e19f30c63eb87ce1907c1511) is the commit in question that most likely solved the issue.

This is a screenshot of the code segment in question that I feel gives me enough information that this commit solved the problem:
<img width="884" height="863" alt="image" src="https://github.com/user-attachments/assets/663cb796-6efe-48bb-b64d-59b71911ccab" />

I say this because getSalvageItem() has a comment saying "@return The item that should get salvaged" while [this](https://[McMMO](https://github.com/mcMMO-Dev/mcMMO).fandom.com/wiki/Salvage) says "Salvage is the ability to reclaim the base materials from tools and armor. It is a child skill of Repair and Fishing, and it is calculated by averaging the two levels together" now. This means it is possible my issue was in consideration at a large scale rework of [McMMO](https://github.com/mcMMO-Dev/mcMMO). I do see several issues such as [this](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/876) and [this](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2350) reported related to SuperBreaker efficiency, but not necessarily anvil/furnace efficiency being removed.

### Was the issue reported before?

Interestingly, there is an issue that was giving an idea on June 28, 2015 [here](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2635) similar to my bug, where [t00thpick1](https://github.com/t00thpick1), the person who fixed my bug and reworked the salvaging system, said "Sorry not happening." This was said despite "Power 7" and "sharpness 6" being mentioned on July 28, 2015. However, this was only posted a month after the June 28, 2015 feature request, so it makes sense that [t00thpick1](https://github.com/t00thpick1) denied it.

<img width="968" height="737" alt="image" src="https://github.com/user-attachments/assets/9a4fe1b4-ccf5-43bb-acc5-09ff7dbbf14f" />

I believe [t00thpick1](https://github.com/t00thpick1) said that because the ideas were too custom in the context of [McMMO](https://github.com/mcMMO-Dev/mcMMO) at a large-scale, while mine was much more simplistic of just allowing salvaging to go further than efficiency 5. Some other issues I found with the keyword "anvil" are [this](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2902) and [this](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2785).

Someone was before me by a year found at [this issue](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2514). However, this covered the "anvil" part, not necessarily the cooking in furnace part that I discovered as well. So my discovery may have been important! See this image of that issue report:

<img width="961" height="503" alt="image" src="https://github.com/user-attachments/assets/f4a0b712-8538-40e8-8f4e-128b9009cdd6" />

The issue was closed the same day as mine. This issue matched 1:1 with [my issue](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/3033).

The other issues relating to "anvil" from before my report on September 18, 2016 appear to not be related to my issue when I glance over the titles. So that means [me](https://github.com/bluelightspirit) and [KET762](https://github.com/KET762) both helped resolve this issue with [McMMO](https://github.com/mcMMO-Dev/mcMMO), and assisted with a large-scale rework. I also cannot find other issues relating to "furnace" from before my report on September 18, 2016 that are related to my issue besides [this](https://github.com/[McMMO](https://github.com/mcMMO-Dev/mcMMO)-Dev/[McMMO](https://github.com/mcMMO-Dev/mcMMO)/issues/2557) that got resolved in 2015 and was not related to efficiency level, but rather lore.

## Conclusion

I ([bluelightspirit](https://github.com/bluelightspirit)) helped resolve a somewhat annoying thing going on with [McMMO](https://github.com/mcMMO-Dev/mcMMO) relating to efficiency not staying whenever an anvil or furnace was used, by reporting the issue on GitHub. I was not the only one to do so, as [KET762](https://github.com/KET762) reported it before me, though they did not mention the furnace part as something else to check with salvaging just in-case. But that is ok! That is what other people are there for, to give different perspectives with their own black box tests and experiences as customers of the product.
