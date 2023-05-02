# Goal of Repository

This repository holds a collection of files which contain the following enhancements for community-made classic Doom addon levelsets, which are known as PWADS:
- Widescreen graphics for menus and title screens (ex: wadnamehere_pics_wide21.wad)
- Widescreen graphics for the status bar HUD (ex: wadnamehere_bar_wide32.wad)
- UMAPINFO definitions to define level names for automap and more, for WADs that did not use DEHACKED for this. (ex: wadnamehere_umapinfo.wad)
- In rare cases, compatability aids if the original /idgames release is too difficult for the average user to apply to a modern sourceport. (ex: wadnamehere_compat.wad)

Many of these enhancements exist around already (other github repos, Doomworld threads, etc.) This repository serves to collect them all into one place.

The graphics files will be denoted by 'wide' (for 16:9 content), 'uwide' (for 21:9 content), 'suwide' (for 32:9 content) or 'gwide' (for even wider HUD content). Only one size will be maintained for each WAD (the widest content submitted.) It is designed to crop down to the aspect ratio your monitor uses.

Each of these items are stored in separate WADs so that a user can easily use only the parts they desire.

The goal of these enhancements is to remain true to the original content of the addons, simply making the graphics fill out today's common widescreen monitors, rather than to try to improve the graphics in general.

# How to Use

These files are designed for modern engine upgrades of Doom, which are called sourceports.

Most modern Doom sourceports, such as Woof!, DSDA-Doom, Crispy Doom, and PrBoom Plus make it easy to use these additions. 
Simply place the 'autoload' folder from this repository into the source port's directory. Then, when you launch the sourceport with a PWAD, it will automatically autoload all of the content from the autoload folder that matches the PWAD's filename. You do not have to explicitly launch the sourceport with 

GZDoom does not (yet?) support this feature. You will have to launch GZDoom explicitly with the appropriate files for the PWAD you want to play.

To best launch a Doom source port with PWADs, consult other programs, such as the Doom launcher [qZDL](https://github.com/lcferrum/qzdl).

# Contribution

To submit graphics to this project, open a Pull Request, or if you don't know how, start an Issue with your content attached as well as any credits.

If you want to contribute to this project, please adhere to these Suggestions and Guidelines.

## Contribution Guidelines
- Graphics must be no taller than the originals. That means pics must be 200px tall, and status bars must be 32px tall.
- I will allow submissions of 4 size categories:
	- wide, meaning 16:9. The bare minimum for inclusion. You are Wide if the images are at least 428 pixels wide.
	- wide21 - 21:9 or "Ultrawide". This is my recommended size. You are wide21 eligible if the images are at least 576 pixels wide.
		- There is a caveat, I will allow pics that are only 560px wide, because most of the existing ultrawide wide content is 560 pixels wide. However, I require all status bars to be at least 576 pixels wide. This is because most 21:9 monitors are not actually a 21:9 aspect ratio but a little bit wider. A status bar of only 560 pixels wide will leave gaps. If you submit 560px wide status bars they will be modified to be 574px.
	- wide32 - 32:9 or "Super Ultrawide". You are wide32 eligible if the images are at least 854 pixels wide. These are super uncommon so I don't really recommend making this but I won't stop you.
	- widex - "Xtra wide" for status bars wider than 1280 pixels. This pretty much only exists to cover GZDoom's hud scaling. Dont go out of your way to make these.
		- I wont bother with widex background pics. Only status bars.
		- I only really have this category because of Eviternity's canon widescreen status bar graphic.
	- I will NOT maintain different versions for different aspect ratios. The widest content of good quality gets to stay.
- Please submit content following the WAD naming scheme explained in the 'Goal of Repository' section.
- I will NOT require that all pixels in the original 320x200 (4:3) space be untouched. However, I strongly encourage it.
	- I WILL require that any text, logos, signatures, etc. that were in the original 320x200 (4:3) space must remain there and not be removed or moved outside of the original 4:3 space.
	- You may modify content in the original 320x200 (4:3) space ONLY for the purpose of blending better with the added content to the sides. However, it MUST still look good if cropped back to 4:3!
- Do not use this as an opportunity to 'improve' the original content. Yes, the Hell Revealed status bar is horiffically garish, etc. But I would like this repository to be as accurate as possible to the original content.
- I won't maintain multiple 'alternate' versions of graphics, I will choose the one I think is best. The only exceptions will be extreme cases such as JPCP's japanese version HUD. 
- If your graphic expands the image by only adding flat black to both sides, do not bother including it. All source ports will do this already to the original graphics.
- If you are uncomfortable with any of the following situations, don't submit it:
	- your work hypothetically being included in a re-release of the wad (be it a new idgames update by the original wad's authors, or perhaps ported to console doom's addons)
	- your work hypothetically being used as a base for other widescreen graphics submissions
	- you submit multiple graphics for the same wad but would be upset if not all of your graphics are used and some are picked from a different submission
  - your work potentially being modified after submission, such as to extend 560px content to 576px, or wide content being extended to uwide.
- Attribution is required. If you base any work off of any graphics other than from the original WAD, please specify the original authors and/or sources so that they may be correctly credited.
	- This means don't submit something you found on a forum or other repository unless you're sure of who made it, and you have reasonable belief that they would be OK with their work being used, modified, or submitted.


## Contribution Suggestions
- In my opinion, status bars are way more important than background images, so I encourage prioritizing them.
	- Menu pics letterboxed in black look way less jarring than status bars that have unmatching screen border textures on each side.
	- You only see the menu pics a few times. You see the status bars the whole time you play.
- Design all graphics as if they could be cropped at ANY random point beyond the original 320 pixel (4:3) space.
	- This will allow all graphics to be suitable for 16:10, 16:9, 21:9 or anywhere in between. 
	- To facilitate this:
		- Try not to put any important objects that might become confusing if cropped in half. For instance a feature at the edge of 16:9 space that could be cropped for 16:10 users.
		- Try not to rely on fancy borders at the edges of your 16:9 or 21:9 graphics. Users of different aspect ratios such as 16:10 may not see it, and in other cases they may be slightly cropped due to rounding errors.
- Don't forget about Doom's Aspect Ratio. Essentially, all graphics are displayed on screen 20% taller than they are in the actual image file. So be careful if for instance you're drawing circles. Account for this or they will become ovals in-game.
