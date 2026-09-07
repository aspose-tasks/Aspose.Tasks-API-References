---
title: "Project.OleObjects"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। OleObject क्लास की उन इंस्टेंसों को शामिल करने वाला संग्रह प्राप्त करता है जो इस प्रोजेक्ट फ़ाइल से लिंक या एम्बेडेड हैं। केवल mpp फ़ाइल फ़ॉर्मेट के लिए उपलब्ध है। यह संग्रह केवल Clear ऑपरेशन को छोड़कर पढ़ने‑के‑लिए‑रोक है।"
type: docs
weight: 700
url: /hi/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

[`OleObject`](../../oleobject/) क्लास की उन इंस्टेंसों को शामिल करने वाला संग्रह प्राप्त करता है जो इस प्रोजेक्ट फ़ाइल से लिंक या एम्बेडेड हैं। केवल mpp फ़ाइल फ़ॉर्मेट के लिए उपलब्ध है। यह संग्रह 'Clear' ऑपरेशन को छोड़कर पढ़ने‑के‑लिए‑रोक है।

```csharp
public OleObjectCollection OleObjects { get; }
```

## उदाहरण

एक एम्बेडेड OLE ऑब्जेक्ट को निकालने का तरीका दर्शाता है।

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### संबंधित देखें

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


