# Platform Overrides for the Analogue Pocket

This repository contains image and JSON overrides I've used for various cores on the Analogue Pocket. You can use them, too, if you'd like. 

I've separated my overrides into two categories: one for `arcade` cores, and a `home` category that contains overrides for consoles, handhelds, and computers. To use these images and overrides simply download a release, or download the entire repository and copy the contents of the Platforms folder into your own Platform folder. Or, pick and choose what you'd like to use. :)

The `pics` directory includes the raw PNG files I used to make the images.  I have them all laid out below so you can take a quick glance at them and determine whether or not your want to use them.

<table>
<tr>
 <th><a href="image_overview_arcade.md">View all Arcade Images</a></th>
 <th>
   <a href="image_overview_home.md">View all Home Images</a><br />
   <a href="image_regional_differences.md">Regional Variants</a>
 </th>
</tr>
<tr>
 <td>
   Examples
   <img src="pics/arcade/garegga.png" />
   <img src="pics/arcade/xevious.png" />
   <img src="pics/arcade/jtcps1.png" />
 </td>
 <td>
   Examples
   <img src="pics/home/snes.png" />
   <img src="pics/home/gba.png" />
   <img src="pics/home/amiga.png" />
 </td>
</tr>
</table>

Enjoy!

Thanks to **<a href="https://github.com/mattpannella">mattpannella</a>** for release details, and **<a href="https://github.com/terminator2k2">terminator2k2</a>** for the repo folder structure.

- Note: There's an `_alternatives` directory that contains previous or alternate overrides you can use with cores.

- Note: There's also an `_unreleased` directory that has overrides for cores that haven't been released yet. These are not included in releases. But, as new cores are completed, they will be moved into the appropriate directories and a new release will be made. If you'd like to get them now, download the whole repository and grab them that way. :)

- Advisory: Putting too many* JSON files in the Platforms folder will caused some problems displaying cores in the openFPGA menu on the Pocket. It's recommended to only use JSON files for cores you have installed.


  - *too many = I don't know the real limit. At one point, I had 310 json in the directory and that was too many. I've also had 100 json in the directory, and that was okay. The limit is probably above 200.

- Also! If you happen to think my images are too graphical and gaudy, then **terminator2k2** has a repo with only logos: <a href="https://github.com/terminator2k2/Analogue-Pocket-Core-Art">here</a>.
