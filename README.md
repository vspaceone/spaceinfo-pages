# spaceinfo-pages

repository for the slides of the spaceinfo-terminals. The server software is described [https://github.com/vspaceone/spaceinfo](here).

## So sieht das bei uns aus:
![Bildschirme im Space](spaceinfo.jpg)

## How to add slides?
To add slides you should add a subfolder in `pages`. But a `config.ini` file into this directory. This file should look like:
```
[Page-Settings]
# If external link is set; The link is used instead of the local index.html file
#external_link = https://www.netzfrequenz.info/charts/gauge_full.php

# If timeout is set; The page will be shown for this time in seconds. If not set, the default timeout will be used
#timeout = 42

# In which slideshow should this page occur?
slideshows = internal maxpriv

# Start and enddate (none is forever)
#startdate = 2018-12-26T00:00:00+01:00
#enddate = 2018-12-31T23:59:59+01:00

```
You need to specifiy either a `external_link` in your `config.ini` or add a `index.html` file to the directory. You could add you slide to multiple `slideshows` by specifying them separated by a space.

You find some templates in the `templates` directory.

Make PullRequest from a branch in THIS repository! :)

## Licence
Siehe [LICENCE](LICENCE.md)
