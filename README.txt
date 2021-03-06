      __                                            __     
    /    )          /          ,        /           /      
----\--------------/__--_/_------_/_---/----__-----/---_/_-
     \     /   /  /   ) /    /   /    /   /___)   /    /   
_(____/___(___(__(___/_(_ __/___(_ __/___(___ _ _/_ __(_ __
                                                           

Ruby tool to download, create, convert and fix subtitles.


== FEATURES:

* To and from: SRT, SUB, XML(TT), YML, MPL2, RSB and ASS.
* Download from opensubtitles.org
* Fixes delays. (SrtResync)
* Compatibility with "sube" (http://github.com/vic/sube)


== TODO:

Please visit:
  
* http://nofxx.lighthouseapp.com/projects/17299-subtitle_it


== REQUIREMENTS:

* hpricot


== SYNOPSIS:

Bash tool:

Convert a srt to sub:
  subtitle_it in.srt out.sub
  or
  subtitle_it -c sub in.srt

Add a delay of 1 minute:
  subtitle_it -d 60 in.srt
 
Create a template
  subtitle_it unexistent.file 
  

== INSTALL:

 gem sources add http://gems.github.com
 sudo gem install nofxx-subtitle_it


== THE "Ruby Subtitle" Format - RSB

It`s just a easy way, proof of concept to edit subtitles. Here is what it looks like:

00:32 => 00:33 == Nice police work! | Thank you!
00:35 => 3 == Nice job!

MM:SS => MM:SS or N == TEXT | NEWLINE

Create a template to check it out. 


== DEV:

To run tests:

  rake spec or autotest
  
Documentation => doc
Subtitle examples => spec/fixtures
  

== SUBTITLE EDITORS:

Try those nice editors too, if SubtitleIt does not fit your need:

Jubler: http://www.jubler.org/

Aegisub: http://www.malakith.net/aegiwiki/Main_Page


== THANKS

* Johanlunds - Opensubtitle.org code (to be used as a gem soon).
* Marcin (tiraeth) Chwedziak - Sub format first implementation.


== LICENSE:

(The MIT License)

Copyright (c) 2008 Marcos Piccinini, Giovanni Rapagnani, Warlley Rezende


Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
