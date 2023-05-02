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

If you want to contribute to this project, please adhere to the [Suggestions and Guidelines](GUIDELINES.md)
