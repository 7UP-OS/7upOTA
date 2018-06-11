7upOTA
-------
A very simple OTA checker with Android Settings look and feel.

How it works
------------
It parses the OTA xml file that you put in your file hosting and compares the version number with the local one.
If the version is newer, it notifies the user for a new ROM update.

### Most guys can skip the below part

Define how 7upOTA should know about the "version". The version must be parseable to a date.
Usually, the version is a part of a build name. For example, the 20150426 in the SlimSaber-bacon-5.0.2-20150426.
Adjust the OTA configuration according to your build name on how should 7upOTA parse the version
Find a key in build.prop that represents the 7up-O-v1.0.0-20180611-a3y17lte-Official.zip and set it in the "version_name"
Set the delimiter in "version_delimiter" to "-"
Set the date format in "version_format" to "yyyyMMdd"
Set the position in "version_position" to "3" (zero based)
Find a key in build.prop that represents your device name and set it in the "device_name"
7upOTA will search this device name in the OTA xml file


Credits
-------
* [SlimRoms team](http://Slimroms.net/)
  * For the original idea of the SlimCenter and app icon
