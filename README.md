# Creating the Meyrin CERN terminal font.

![Meyrin Terminal Font](http://i.imgur.com/doCoEa3.png)

The process is pretty straight-forward. It is a two step processes. First you need to create an SVG file for each glyph. There is a template.svg which can be used to create new glyphs. There is a descender of two units and ascender of 3 units. This is used for diacritics.

Once each glyph is an individual SVG file, you can import them into a font creation tool. We used the online service http://icomoon.io From this we upload and map each SVG file to a specific unicode code point. We did some final tweaks in font forge to get the space character and additional metadata. 

We completed all the characters which are available on the IBM System 6000 keyboard. We ran a simple script to output all available characters, took screenshots and tried to create these as well. This is not a complete Unicode font, but you are welcome to fork the repo and create additional glyphs as needed.