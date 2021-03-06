# Equirectangular local images viewer for Qgis

This plugin allows the visualization of equirectangular local images, although modifying the code, it can be used for any 360 image, given that the library [Marzipano](https://github.com/google/marzipano) is used.
 
[Example](https://github.com/All4Gis/EquirectangularViewer/tree/master/example)
 
## Prerequisites
 
The libraries [CefPython](https://github.com/cztomczak/cefpython) is required, you can find them in:
- [x86](https://github.com/All4Gis/EquirectangularViewer/tree/master/ext-libs/x86/cefpython3)
- [x64](https://github.com/All4Gis/EquirectangularViewer/tree/master/ext-libs/x64/cefpython3)

These libraries must be placed in `D:\OSGeo4W64\apps\Python27\Lib\site-packages ` or something similar depending on your Qgis installation.
 
On the other hand, the plugin must be placed in the `.qgis` path, it should be something like   `C:\Users\<username>\.qgis2\python\plugins `
 
Once installed, you can test the correct functioning of the plugin with the example that is provided,a shapefile with some images.
 [.shp](https://github.com/All4Gis/EquirectangularViewer/tree/master/Shapefile)
 
## How it works?
 
It’s simple:
- You start a local server in Python in  `http://127.0.0.1:1520/viewer.html `
- A copy of the image associated to the selected registry is created in the folder where our viewer and server are.
- With cefpython, we open the browser and return the current yaw to our canvas anytime the image is moved.
 
 
## Donations
Want to buy me a beer (or gadget)? Please use Paypal button on the project page,[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/all4gis), or contact me directly.

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?button=donate&business=5329N9XX4WQHY&item_name=EquirectangularViewer+Plugin&quantity=&amount=&currency_code=EUR&shipping=&tax=&notify_url=&cmd=_donations&bn=JavaScriptButton_donate&env=www)
 
If this plugin is useful for you, consider to donate to the author.

[© All4gis 2017]
