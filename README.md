
# PowerApps-SVG-Merge-Modul

`EN`
Merge multiple images seamlessly in PowerApps without the need for any complex coding or external components. With the easy-to-use 🎨 Over Layer Settings, you can easily adjust the order of any layers, while the ✍️ Over Text Settings lets you add and position text over the arrows with or without a bounding box. The result is a high-quality 🌟*.SVG image that you can download.

`DE`
Fügen Sie Bilder in PowerApps nahtlos zusammen, ohne auf komplexe Codierung oder externe Komponenten angewiesen zu sein. Mit den einfachen 🎨 Over-Layer-Einstellungen können Sie die Reihenfolge der Ebenen anpassen, während Sie mit den ✍️ Over-Text-Einstellungen Texte mit und ohne Begrenzungsrahmen hinzufügen und die Position der Texte über die Pfeile ändern können. Das Ergebnis wird in einer hochwertigen 🌟*.SVG-Datei generiert, die Sie herunterladen können.

**Erhöhte Flexibilität durch "FileContent" und "SVG Raw" im Konvertierungsprozess**

Die Verwendung von "FileContent" und "SVG Raw" in unserem Konvertierungstool bietet eine erhöhte Flexibilität und ermöglicht es uns, SVG-Dateien nahtlos in andere Formate umzuwandeln und sie vielseitig für verschiedene Zwecke einzusetzen. Diese Funktionen eröffnen uns eine Vielzahl von Möglichkeiten, um unsere SVG-Dateien effektiv zu verarbeiten und sie optimal in unseren Projekten zu nutzen.

**"SVG Raw" - Unveränderter SVG-Code**

"SVG Raw" enthält den unkonvertierten, unveränderten SVG-Code. Mit dieser Funktion haben wir direkten Zugriff auf den ursprünglichen Inhalt unserer SVG-Datei. Dadurch können wir die SVG-Datei bei Bedarf direkt und ohne Veränderungen verwenden. 📄🔍

**"FileContent" - Data URI-Struktur**

Die Struktur eines Data URI besteht aus dem Schema "data:", gefolgt von einem Medientyp (z. B. "text/plain" für Text oder "image/svg+xml" für SVG-Bilder), einem optionalen Zeichensatz und den eigentlichen Daten, die codiert und in Base64 umgewandelt werden.

## Image Generator Properties

#### Input

- **Image Name**
  - Type: String
  - Default: Blank
  - Description: Image Name for File Name

- **Image Background**
  - Type: Image
  - Default: Sample Image
  - Description: Default Background Image

- **Output Image Size**
  - Type: Record (Integers)
  - Default: {Width:640, Height:640}
  - Description: Image Output Size

- **Custom Title**
  - Type: String
  - Default: $"Sample_{RandBetween(1,123456)}"
  - Description: Image Name for File Name without Extension

- **Image Background Position**
  - Type: Enum
  - Default: ImagePosition.Fit
  - Description: Image Background Position

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
  - Description: Show Menuicons

- **Text Colors**
  - Type: Array
  - Default: List of Colors
  - Description: Colorlist for Text

- **Arrow Pressed Color**
  - Type: Color
  - Default: RGBA(243, 139, 66, 1)
  - Description: Text Arrows Pressed Color

- **Menu Icon Size**
  - Type: Integer
  - Default: 60
  - Description: Menu Icon Size

- **Original Image Size**
  - Type: Boolean
  - Default: false
  - Description: use the Original Image Size as Output Size

#### Output

- **Generated Output Data**
  - FileName (Filename with Extension)
  - FileSize (Image Size like 640x640)
  - FileContent (Data URI Schema)
  - RawContent (RAW SVG File)
  - File (Generated File for z. B. Verwendung im Attachment Control)
  - Schema: { Name: "", Value: "" }


## Video

https://github.com/mlnc21/PowerApps-SVG-Merge-Modul/assets/80674540/d096e6ee-9208-49b5-b75b-3bbae3e73f1c



## Features
- Convert SVG to JPG
- Generate SVG RAW + File Content (Name,Value)
- Pen Color Control
- Pen Size Control
- Text Control
- Layer Control

## Minimal Path to Awesome

* [Download](SVGMergeModulExample.zip) the `.zip`
* Within **make.powerapps.com**, use the `.zip` file using **App** > **Import Canvas App**  and select the `.zip` file you just downloaded.
* Select the **Upload** Button

* Give your Uploaded `.zip` a **AppName** and **Import** the App.

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**
