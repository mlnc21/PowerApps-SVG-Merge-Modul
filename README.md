# PowerApps SVG Merge Module

Merge multiple images in PowerApps without complex code or external components.  
Use the layer settings to control the order of elements, and the text settings to place text on top of arrows with or without a background box. The result is a high-quality SVG image that you can download or use in your app.

## File content options

This solution supports two useful output formats:

- **SVG Raw**: the original SVG code without changes
- **FileContent**: a Data URI version of the SVG content, encoded in Base64

These formats make it easier to reuse the generated image in different scenarios.

## Image Generator Properties

### Input

- **Image Name**
  - Type: String
  - Default: Blank
  - Description: Name of the exported file

- **Image Background**
  - Type: Image
  - Default: Sample Image
  - Description: Background image used in the output

- **Output Image Size**
  - Type: Record (Integers)
  - Default: `{Width: 640, Height: 640}`
  - Description: Size of the generated image

- **Custom Title**
  - Type: String
  - Default: `$"Sample_{RandBetween(1,123456)}"`
  - Description: File name without extension

- **Image Background Position**
  - Type: Enum
  - Default: `ImagePosition.Fit`
  - Description: How the background image is placed

- **Offset Background**
  - Type: Record (Integers)
  - Default: `{OffsetX: 0, OffsetY: 0}`
  - Description: Background offset

- **Offset Pen**
  - Type: Record (Integers)
  - Default: `{OffsetX: 0, OffsetY: 0}`
  - Description: Pen offset

- **Show Extended Control**
  - Type: Boolean
  - Default: `true`
  - Description: Shows additional menu icons

- **Text Colors**
  - Type: Array
  - Default: List of colors
  - Description: Available text colors

- **Arrow Pressed Color**
  - Type: Color
  - Default: `RGBA(243, 139, 66, 1)`
  - Description: Color used when an arrow is pressed

- **Menu Icon Size**
  - Type: Integer
  - Default: `60`
  - Description: Size of the menu icons

- **Original Image Size**
  - Type: Boolean
  - Default: `false`
  - Description: Uses the original image size as the output size

- **Rotate Background**
  - Type: Number
  - Default: `0`
  - Description: Rotates the background image by a given angle, for example 90, 180, or 270 degrees

### Output

- **Generated Output Data**
  - **FileName**: file name including extension
  - **FileSize**: image size, for example `640x640`
  - **FileContent**: SVG content as a Data URI
  - **RawContent**: raw SVG file data
  - **File**: generated file for use in controls such as Attachment Control
  - **Schema**: `{ Name: "", Value: "" }`

## Features

- Convert SVG to JPG
- Generate SVG Raw and FileContent output
- Control pen color
- Control pen size
- Control text
- Control layers
- Rotate the background image and individual photo layers

## Quick Start

1. Download the [`SVGMergeModulExample.zip`](SVGMergeModulExample.zip) file.
2. Open **make.powerapps.com**.
3. Go to **App** > **Import Canvas App** and select the downloaded ZIP file.
4. Click **Upload**.
5. Enter a name in **AppName** and finish the import.

## Video Demonstrations

![Demo 1](https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/blob/731fa7de6781959fcd194fc9e766ee6c7925e5be/Videos/Demo_1.gif)
![Demo 2 with Background Image](https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/blob/731fa7de6781959fcd194fc9e766ee6c7925e5be/Videos/Demo_2.gif)

## FAQ

### How do I fix the component behavior property return type check issue?

You can solve this in two ways:

1. **Disable the retired feature**
   - Open the app.
   - Go to **Settings** > **Updates** > **Retired**.
   - Disable **Disable component behavior property return type check**.

2. **Use `IfError`**
   - Wrap the affected action in `IfError` to handle the return type safely.

## Disclaimer

**THIS CODE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**
