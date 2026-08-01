# Platform Overrides for the Analogue Pocket

This repository contains image and JSON overrides I've used for various cores on the Analogue Pocket. You can use them, too, if you'd like. 

I've separated my overrides into two categories: one for `arcade` cores, and a `home` category that contains overrides for consoles, handhelds, and computers. There are two additional home directories, `home-jp` and `home-pal` that contain different images for regional variants. To use these images and overrides simply download a release, or download the entire repository and copy the contents of the Platforms folder into your own Platform folder. Or, pick and choose what you'd like to use. :)

The `pics` directory includes the raw PNG files I used to make the images.  I have them all laid out below so you can take a quick glance at them and determine whether or not your want to use them.

<table>
<tr>
 <th><a href="/image_overview_arcade-all.md">View all Arcade Images</a></th>
 <th><a href="/image_overview_home.md">View all Home Images</a></th>
</tr>
<tr>
 <td>
   Examples
   <img src="/pics/arcade/garegga.png" />
   <img src="/pics/arcade/jtcastle.png" />
   <img src="/pics/arcade/xevious.png" />
 </td>
 <td>
   Examples
   <img src="/pics/home/snes.png" />
   <img src="/pics/home/gba.png" />
   <img src="/pics/home/amiga.png" />
 </td>
</tr>
<tr>
 <th></th>
 <th><a href="/docs/image_regional_variants.md">Regional Variants</a></th>
</tr>
<tr>
 <td>
   More Arcade Examples
   <img src="/pics/arcade/jtcps2.png" />
   <img src="/pics/arcade/jts16_c.png" />
 </td>
 <td>
   Examples
   <img src="/pics/home-pal/snes.png" />
   <img src="/pics/home-jp/pcecd.png" />
 </td>
</tr>
</table>

Enjoy!

Thanks to **<a href="https://github.com/mattpannella">mattpannella</a>** for release details, and **<a href="https://github.com/terminator2k2">terminator2k2</a>** for the repo folder structure.

- Note: There's an `_alternatives` directory that contains previous or alternate overrides you can use with cores.

- Note: There's also an `_unreleased` directory that has overrides for cores that most likely won't be released. These are not included in the releases. But, if these cores eventually are released, they will be moved into the appropriate directories and a new release will be made. If you'd like to get them now, download the whole repository and grab them that way. :)

- **Advisory**: Overall, there is a significant amount of images and overrides in each release of pocket-images. You can copy over all of the images, but it's recommended to only use JSON files for cores you have installed. Putting too many JSON files in the Platforms folder will cause openFPGA to not function. 

How many is 'too many'?? Please read the following:

## Disclaimer about Too Many Platforms

When there are too many JSON files in the Platforms folder, the Pocket will begin having errors trying to display everything. It has been determined that 239 cores is the general limit, but there is some wiggle room both ways depending on what cores you have installed. Once you hit your limit, openFPGA will display a QR code saying things are broken. You have too many cores.

It is now August 1st 2026, and there are more than 239 cores available to the public. You can't have absolutely everything available all at once. However, you can have everything installed if you like..

<a href="https://github.com/neil-morrison44/pocket-sync">Pocket Sync</a> and <a href="https://github.com/mattpannella/pupdate">Pupdate</a> are you friendly neighborhood Pocket updaters. By using them, you can see everything you have installed, everything available you don't have installed, and you can download my images through them, too. Because of the platform limit, they've added an option to 'archive' cores. Archiving a core moves the platform json out of its directory, but keeps all the core contents intact. They won't show up in openFPGA, but you can easily unarchive the core and have it available again.

<b>I recommend using the updaters to manage your favorite cores and prevent your Pocket from hitting the platform limit.</b>

## Combo Cores

There's another option to help reduce your number of cores: <b>You can use combination cores.</b> Several Arcade cores have been released that only load a single game, even though the architecture of the hardware is the same or near the same as another single Arcade core. As long as the video options are the same, you can make some alterations to the core's JSON setup and have the core run different RBF builds depending on the games you choose.

There are already a few combination cores that Espiox and myself have put together.
- <b>Sega System 16 Combo</b> combines System 16A and System 16B together. Details are <a href="https://github.com/espiox/jts16_complete">here</a>.
- <b>Williams 6809 Combo</b> combines Defender, Robotron, and Joust 2 cores together. Details are <a href="https://github.com/dyreschlock/pocket-extras/tree/main/williams_complete">here</a>.
- <b>Capcom Z80 Combo</b> combines 1942, 1943, Black Tiger, Commando, Exed Exes, Gun.Smoke, Section Z, Legendary Wings, Trojan, and Hyper Dyne Side Arms together. Details are <a href="https://github.com/dyreschlock/pocket-extras/tree/main/jtcz80_combo">here</a>
- <b>Toaplan V2 Hardware Combo</b> combines Garegga, Bakraid, Soccer Strike, Kingdom Grand Prix, Armed Police Batrider, Snow Bros 2, Truxton 2, Pipi & Bibs, and Teki Paki cores together. Details are <a href="https://github.com/dyreschlock/pocket-extras/tree/main/toaplan2_complete">here</a> 
- <b>Toaplan V1 Hardware Combo</b> combines Demon's World and Zero Wing. Preliminary details are <a href="https://github.com/dyreschlock/pocket-extras/tree/main/toaplan1_complete">here</a>

Using all 5 of these Combo cores will save you 21 platforms. All of these combination cores are available through <a href="https://github.com/mattpannella/pupdate">Pupdate</a>, so you don't need to worry about any complicated instructions.

There are two drawbacks for doing this that I can think of. 1. It can sometimes make finding specific games more difficult if you don't know where to look. 2. Automatic Pupdates are now dependent on the authors of these Combo cores updating their repos after the main repos are updated. I am not good at this.