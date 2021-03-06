OpenLayers v2
=============

Shim repository for [OpenLayers](http://openlayers.org/two/).

Copyright (c) 2005-2015 OpenLayers Contributors. See authors.txt for more details.

OpenLayers is a JavaScript library for building map applications on the web. OpenLayers is made available under a BSD-license. Please see license.txt in this distribution for more details.

Package Managers
----------------

* [Composer](https://getcomposer.org/): `philvanbwg/openlayers`

## Getting OpenLayers 2

OpenLayers lives at http://www.openlayers.org/two/.  Find details on downloading stable releases or the development version the [development site](http://trac.osgeo.org/openlayers/wiki/HowToDownload).

## Installing OpenLayers 2

You can use OpenLayers as-is by copying build/OpenLayers.js and the
entire theme/ and img/ directories up to your webserver and putting them
in the same directory. The files can be in subdirectories on your website,
or right in the root of the site, as in these examples.
To include the OpenLayers library in your web page from the root of the site, use:

    <script type="text/javascript" src="/OpenLayers.js" />

As an example, using bash (with the release files in ~/openlayers):

    $ cd /var/www/html
    $ cp ~/openlayers/OpenLayers.js ./
    $ cp -R ~/openlayers/theme ./
    $ cp -R ~/openlayers/img ./

If you want to use the multiple-file version of OpenLayers (for, say,
debugging or development purposes), copy the lib/ directory up to your
webserver in the same directory you put the img/ folder. Then add
the following to your web page instead:

    <script type="text/javascript" src="/lib/OpenLayers.js" />

As an example, using bash (with the release files in ~/openlayers):

    $ cd /var/www/html
    $ cp -R ~/openlayers/lib ./
    $ cp -R ~/openlayers/theme ./
    $ cp -R ~/openlayers/img ./

## Alternate OpenLayers 2 Versions in this Release

The following versions of OpenLayers 2 single file builds are included in this release
and can be used in place of OpenLayers.js in any of the above instructions:

1. OpenLayers.js - full build --> Includes everything except the alternate language
    translations and deprecated classes.
2. OpenLayers.mobile.js - a mobile focused build --> Includes a subset of the OpenLayers 2
    library to serve common mobile web app use cases. This build provides access to
    OpenStreetMap, Bing, WMS, WFS and vector layers; touch optimized controls; geolocation;
    vector editing and interaction tools. The examples tagged ``mobile`` can use this build.
3. OpenLayers.light.js - a simple use case focused build --> Includes a subset of the
    OpenLayers library to serve the basic use case of displaying points and polygons
    on a map. This build provides access to OpenStreetMap, Bing, Google, WMS, and
    vector layers; basic map controls; and vector interaction tools. The examples
    tagged ``light`` can use this build.

## Using OpenLayers 2 in Your Own Website

The [examples directory](http://dev.openlayers.org/examples/) is full of useful examples.

Documentation is available at http://trac.osgeo.org/openlayers/wiki/Documentation.
You can generate the API documentation with http://www.naturaldocs.org/
As an example, using bash (with the release files in ~/openlayers):

    $ cd ~/openlayers/
    $ /path/to/NaturalDocs -i lib/ -o HTML doc/ -p doc_config/ -s Default OL

Information on changes in the API is available in release notes found in the notes folder.

## Contributing to OpenLayers 2

Please join the email lists at http://trac.osgeo.org/openlayers/wiki/MailingLists
Patches are welcome!

