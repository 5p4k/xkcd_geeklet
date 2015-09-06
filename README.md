About
=====
An xkcd Geeklet that displays the last comic, with title and alt text on your desk.

![Example geeklet](https://cloud.githubusercontent.com/assets/3787759/9703808/fa8e6218-548e-11e5-8586-c1aea1ca1847.png)
*xkcd [comic #1573](http://xkcd.com/1573/), released under [Creative Commons Attribution-NonCommercial 2.5 License](http://creativecommons.org/licenses/by-nc/2.5/).*

Prerequisites
-------------
Python 3.2 (`urllib.request` and `argparse`).

Installation
------------
The Geeklets invoke the xkcd script via
    `/opt/local/bin/python /usr/local/bin/xkcd <args>`
This because I am using MacPorts's Python, and I have symlinked `xkcd` to `/usr/local/bin`. Edit the Geeklets according to your configurations.

Usage
-----
By default, xkcd comic data are stored in `/tmp/xkcd.png` and `/tmp/xkcd.json`.

Crash course:
  - __Download a comic:__ `xkcd --remote <comic num>`
  - __Download latest comic:__ `xkcd --remote`
  - __Automatically refresh GeekTools:__ append `--update` to the xkcd command.
  - __Extract attributes:__ `xkcd --remote <optional num> --get <attrib>` or `xkcd --local --get <attrib>` to load the currently cached comic. To see the list of available attributes call `xkcd --help`.

Autor: @5p4k