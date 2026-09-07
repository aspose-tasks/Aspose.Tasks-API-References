---
title: "क्लास OleObjectCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.OleObjectCollection क्लास। OleObject क्लास के उदाहरणों को सम्मिलित करने वाला संग्रह दर्शाता है।"
type: docs
weight: 1130
url: /hi/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

[`OleObject`](../oleobject/) क्लास के उदाहरणों को सम्मिलित करने वाला संग्रह दर्शाता है।

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | संग्रह को साफ़ करता है। इन परिवर्तनों को स्थायी बनाने के लिए project.Save को नए MPPSaveOptions { WriteViewData = true; } के साथ बुलाया जाना चाहिए। |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | `OleObjectCollection` क्लास के उदाहरण को उन [`OleObject`](../oleobject/) क्लास के उदाहरणों को सम्मिलित करने वाली सूची में परिवर्तित करता है। |

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

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


