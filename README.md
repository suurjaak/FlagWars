Flag Wars
=========

Flag Wars (*lipukaardid* in Estonian) was a fairly popular game in parts of
Soviet Estonia. As such cards were not produced by any Soviet manufacturer, and
colour printing was not easily available to the general public, kids drew the
cards themselves. Some even cut flags out of books and glued them on.

My own hand-drawn set, from around 1992:

![Hand-drawn deck](https://raw.github.com/suurjaak/FlagWars/gh-pages/images/th_handmade.jpg)

Print-ready HTML generated from Wikipedia data, 2014:

![Printable deck](images/th_generated.png)

Online generator, print-ready PDFs and HTML content at 
http://suurjaak.github.com/FlagWars/.


Gameplay
--------

In general, very similar to [War](http://en.wikipedia.org/wiki/War_(card_game)).

**Play:** Shuffle and deal all cards. Player next to dealer leads the first round.

**Each round:** Leader announces a field from their topmost card. 
Player with the best score puts the trick under their deck and leads the next round. 
If a player's card has no value in chosen field, leader must choose another field.

**Compare:** Higher numbers are better, except for obesity rate.
If best values are equal, tied players include their next card.

**Endgame:** With 3 cards or less, player can choose which card to use.

**Game over:** When one player loses all cards. Or when last player remains.


Generating
----------

Generator is a single stand-alone HTML page, using embedded JavaScript to 
retrieve the country list from Wikipedia and make a number of separate
queries to assemble card data: reading statistics from country and capital
pages, counting colours in flag and coat-of-arms images.

When generating is complete, the resulting deck can be printed immediately,
or saved to a file on your computer. File can be saved with embedded images,
making it completely stand-alone and not dependent on online Wikipedia.

The number of flag/heraldic colours is blindly parsed from SVG image data,
counting every colour value from image vector attributes. As some image vectors
are crafted quite intricately, numbers can get absurdly large.

Works best in Chrome and Firefox. Printing is crude in Safari and Opera;
Internet Explorer has poor performance in general.


Attribution
-----------

Card generator uses jQuery, http://jquery.com.

Images and most data from Wikipedia.

Obesity data from CIA World Factbook 2008,
https://www.cia.gov/library/publications/the-world-factbook/rankorder/2228rank.html.

Obesity data for Estonia from "Obesity, impaired glucose regulation, metabolic 
syndrome and their associations with high-molecular-weight adiponectin levels" 
by Triin Eglit, 2014-02-14, http://dspace.utlib.ee/dspace/handle/10062/37323.


License
-------

Copyright (C) 2014 by Erki Suurjaak.
Released under the MIT License (see [LICENSE.md](LICENSE.md) for details).
