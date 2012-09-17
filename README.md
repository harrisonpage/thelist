thelist
=======

Show upcoming San Francisco Bay Area concerts via iTunes export and The List.

Ingredients
===========

- An iTunes Library.XML file
- The List

Prerequisites
=============

- Perl 5
- WWW::Mechanize
- Mac::iTunes::Library

Generating iTunes XML File
==========================

As of iTunes 10, select Export library... from the File menu and save the XML file somewhere.

Best Practice Installing Required Perl Modules
==============================================

Use the cpan tool like so: 

    sudo cpan install WWW::Mechanize Mac::iTunes::Library

Example
=======

    ./thelist --file=/tmp/Library.xml --verbose --format=text

Options
=======

Print debug output with the --verbose option.

Specify the path to your Library.xml file with --file. If not specified, environment variable ITUNES_XML will be used.

By default, output will appear in plaintext. You can generate HTML like so: --format=html

One can specify an alternate show/scene page with the --url option.

To Do
=====

- Test under Windows. 
- Test alternate show/scene pages.
- Find AppleScript to automate XML generation.

References
==========

- http://www.calweb.com/~skoepke/
- http://www.foopee.com/punk/the-list/
- http://search.cpan.org/dist/WWW-Mechanize/
- http://search.cpan.org/~dinomite/Mac-iTunes-Library-1.0/

Author
======

- Harrison Page <harrisonpage@gmail.com>
- https://github.com/harrisonpage/thelist
- 17-Sep-2012
