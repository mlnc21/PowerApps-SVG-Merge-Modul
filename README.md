
# PowerApps-SVG-Merge-Modul

Merge multiple images seamlessly in PowerApps without the need for complex coding or external components. With the easy-to-use 🎨 Over Layer Settings, you can easily adjust the order of layers, while the ✍️ Over Text Settings allow you to add and position text over the arrows with or without a bounding box. The result is a high-quality 🌟*.SVG image that you can download.

**Increased flexibility with "FileContent" and "SVG Raw" in the conversion process**

Using "FileContent" and "SVG Raw" in our conversion tool provides increased flexibility, allowing us to seamlessly convert SVG files into other formats and use them for various purposes. These features open up a wide range of possibilities for effectively processing our SVG files and utilizing them optimally in our projects.

**"SVG Raw" - Unmodified SVG code**

"SVG Raw" contains the unconverted, unmodified SVG code. With this feature, we have direct access to the original content of our SVG file, allowing us to use the SVG file directly and without any modifications when needed. 📄🔍

**"FileContent" - Data URI structure**

The structure of a Data URI consists of the schema "data:", followed by a media type (e.g., "text/plain" for text or "image/svg+xml" for SVG images), an optional character set, and the actual data, which is encoded and converted to Base64.

## Image Generator Properties

#### Input

- **Image Name**
  - Type: String
  - Default: Blank
  - Description: Name of the image for the file name

- **Image Background**
  - Type: Image
  - Default: Sample Image
  - Description: Default background image

- **Output Image Size**
  - Type: Record (Integers)
  - Default: {Width:640, Height:640}
  - Description: Size of the output image

- **Custom Title**
  - Type: String
  - Default: $"Sample_{RandBetween(1,123456)}"
  - Description: Name of the image for the file name without extension

- **Image Background Position**
  - Type: Enum
  - Default: ImagePosition.Fit
  - Description: Position of the image background

- **Offset Background**
  - Type: Record (Integers)
  - Default: {OffsetX:0, OffsetY:0}
  - Description: Possibility to set an offset

- **Offset Pen**
  - Type: Record (Integers)
  - Default: {OffsetX:0, OffsetY:0}
  - Description: Possibility to set an offset

- **Show Extended Control**
  - Type: Boolean
  - Default: true
  - Description: Show menu icons

- **Text Colors**
  - Type: Array
  - Default: List of colors
  - Description: Color list for text

- **Arrow Pressed Color**
  - Type: Color
  - Default: RGBA(243, 139, 66, 1)
  - Description: Color of the text arrows when pressed

- **Menu Icon Size**
  - Type: Integer
  - Default: 60
  - Description: Size of the menu icons

- **Original Image Size**
  - Type: Boolean
  - Default: false
  - Description: Use the original image size as the output size

#### Output

-- **Generated Output Data**
  - FileName: The filename with its extension
  - FileSize: The size of the image (e.g., 640x640)
  - FileContent: The data in URI schema format
  - RawContent: The raw SVG file data
  - File: The generated file (e.g., for use in Attachment Control)
  - Schema: { Name: "", Value: "" }

## Video Demonstrations

![Demo1](https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/blob/731fa7de6781959fcd194fc9e766ee6c7925e5be/Videos/Demo_1.gif)
![Demo 2 with Background Image](https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/blob/731fa7de6781959fcd194fc9e766ee6c7925e5be/Videos/Demo_2.gif)

## Features
- Convert SVG to JPG
- Generate SVG RAW + File Content (Name, Value)
- Control pen color
- Control pen size
- Control text
- Control layers

## Quick Start Guide

* [Download](SVGMergeModulExample.zip) the `.zip` file
* Go to **make.powerapps.com**, use the `.zip` file via **App** > **Import Canvas App** and select the `.zip` file you just downloaded.
* Click the **Upload** button
* Name your uploaded `.zip` file under **AppName** and **Import** the app.

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**
