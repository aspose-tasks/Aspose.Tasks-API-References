---
title: "एनम SaveFileFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.SaveFileFormat एनम। प्रोजेक्ट फ़ॉर्मेट चयन के लिए सहेजने की एन्यूमरेशन"
type: docs
weight: 2180
url: /hi/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

प्रोजेक्ट फ़ॉर्मेट चयन को सहेजने के लिए एन्यूमरेशन।

```csharp
public enum SaveFileFormat
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Mpp | `0` | MPP फ़ॉर्मेट। |
| Xml | `1` | XML फ़ॉर्मेट। |
| Html | `2` | HTML फ़ॉर्मेट। |
| Bmp | `3` | BMP फ़ॉर्मेट। |
| Png | `4` | PNG फ़ॉर्मेट। |
| Jpeg | `5` | JPEG फ़ॉर्मेट। |
| Pdf | `6` | PDF फ़ॉर्मेट। |
| Tiff | `7` | TIFF फ़ॉर्मेट। |
| Xps | `8` | XPS फ़ॉर्मेट। |
| Xaml | `9` | XAML फ़ॉर्मेट. |
| Svg | `10` | SVG फ़ॉर्मेट. |
| Csv | `11` | CSV फ़ॉर्मेट. |
| Txt | `12` | टेक्स्ट फ़ॉर्मेट (टैब डिलिमिटेड). |
| Spreadsheet2003 | `13` | स्प्रेडशीट XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml फ़ॉर्मेट. |
| PrimaveraXer | `16` | Primavera PM XER फ़ॉर्मेट. |
| Mpx | `17` | MPX फ़ॉर्मेट. |
| GdHtml | `18` | प्रोजेक्ट डेटा को एक सेट html टेबल्स में सहेजने के लिए Html फ़ॉर्मेट। |

## उदाहरण

दिखाता है कि CSV फ़ॉर्मेट में प्रोजेक्ट को कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


