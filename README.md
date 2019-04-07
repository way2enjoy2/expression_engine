# Way2Enjoy ExpressionEngine Add-on

![version 3.0.0](https://img.shields.io/badge/version-3.0.0-blue.svg)
![supports ExpressionEngine 5.1.3](https://img.shields.io/badge/supports-ExpressionEngine%205.1.3-green.svg)

Visit [Way2ENJOY](https://way2enjoy.com/) for more information.

## Installation

1. [Sign up](https://way2enjoy.com/developers) for the Developer API and get your API key
2. [Download](https://github.com/way2enjoy2/expression_engine/releases) the zip file
3. Create the directory **way2enjoy** in /system/expressionengine/third_party/
4. Upload the files into the new directory
5. Login to ExpressionEngine
6. Click **Developers** -> **Add-Ons**
7. Click **Install** on the Way2ENJOY row
8. Click **Settings** on the Way2ENJOY row
9. Enter your **TingPNG API Key** and click **Save Settings**
10. You're done

Any image you upload will be made smaller with Way2ENJOY. Your original file will be stored
in a folder called **_original**. You can still use your original file if you wish.

## Example usage

To use the Way2ENJOY version of the image.

    {exp:channel:entries channel="pages" limit="1"}
        <img alt="{title}" src="{image}" />
    {/exp:channel:entries}

The tinified version of the image below is 206KB.

![Way2ENJOY version](samples/after.png)

To use the original image.

    {exp:channel:entries channel="pages" limit="1"}
        <img alt="{title}" src="{image:original}" />
    {/exp:channel:entries}

The original image is 1.6MB.

![Original version](samples/before.png)

## Change Log

### Version 3.0.0

February 5th, 2019

* Added [LICENSE.md](LICENSE.md)
* Checked support for ExpressionEngine 5.1.3

As far as we can tell it works fine with ExpressionEngine 5.1.3. We are going to
bump the MAJOR version number like ExpressionEngine did when they re-released ee
with a new license.

### Version 2.0.0

December 4th, 2017

Added support for ExpressionEngine 4.0.

### Version 1.0.3

April 15th, 2015

Bug Fixes:

* EE was showing an error when uploading a file that already existed.

### Version 1.0.2

March 27th, 2015

Bug Fixes:

* EE was showing the filesize of the original image.

General Changes:

* Site ID was set to one. It now uses $data["site_id"] to get the site id.

### Version 1.0.0

March 24, 2015

Initial release

## photo credit

Photo by [Levi Bare](https://unsplash.com/photos/xCfHL21VpDk?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
on
[Unsplash](https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText).
