---
title: "OleObjectCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OleObjectCollection विधि. OleObjectCollection क्लास की इंस्टेंस को OleObject क्लास की इंस्टेंसों वाली सूची में परिवर्तित करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

[`OleObjectCollection`](../) क्लास की इंस्टेंस को [`OleObject`](../../oleobject/) क्लास की इंस्टेंसों वाली सूची में परिवर्तित करता है।

```csharp
public List<OleObject> ToList()
```

### रिटर्न वैल्यू

[`OleObjectCollection`](../) क्लास की इंस्टेंस को सूची में परिवर्तित किया गया, जिसमें [`OleObject`](../../oleobject/) क्लास की इंस्टेंसें शामिल हैं।

## उदाहरण

OLE ऑब्जेक्ट्स के संग्रह के साथ काम करने का तरीका दिखाता है।

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// इंडेक्स एक्सेस का उपयोग करके
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// या enumeration के माध्यम से OLE ऑब्जेक्ट्स पर इटरेट किया जा सकता है
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### संबंधित देखें

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


