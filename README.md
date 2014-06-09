blinkot
=======

Blinkot is a decentralized, democratized, and robust way to collect and distribute short-form information.

Think of a blinkot as somewhere between a tweet and a blog post that anyone can edit and re-share with their changes.

- - - - - - - - - - - - - - - -

Say hello to Blinkot! :)
--
In a nutshell, a blinkot is a simple way to embed 
arbitrary HTML in a URL-contained wrapper that can 
be easily shared.

Requiring the link to remain < 2048 characters
allows it to be posted on most social media sites
and URL shorteners with minimal overhead.
This leads to ~1440 characters of content.

Inherent in each blinkot is also the ability to
modify and create new blinkots. Since the content
is contained in the URL's hash ("#..."), no data
needs to be transferred to the minimalistic site
hosting the blinkot's viewer/editor code.


URL Structure
--
The URL's hash has 4 parts and looks like this...

    http://.../#TITLE_THEME_CONTENTTYPE_CONTENT_DATE
    TITLE:       base64 encoded title text
    THEME:       single letter (l,d)   - see: themeNames
    CONTENTTYPE: single letter (h,r,t) - see: typeNames
    TITLE:       base64 encoded content text
    DATE:        base32 -- new Date().getTime().toString(32);

- - - - - - - - - - - - - - - -
 
Open Source
--
Blinkot is released as open source under The MIT License (MIT).


