---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraXmlReader कंस्ट्रक्टर। PrimaveraXmlReader क्लास का नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

एक नया उदाहरण प्रारंभ करता है [`PrimaveraXmlReader`](../) क्लास का।

```csharp
public PrimaveraXmlReader(string templatePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| templatePath | स्ट्रिंग | टेम्प्लेट का पथ जहाँ Primavera Xml प्रोजेक्ट या प्रोजेक्ट्स स्थित हैं |

## उदाहरण

एक Primavera XML फ़ाइल से छोटे प्रोजेक्ट्स की जानकारी की जांच कैसे करें, यह दिखाता है।

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### संबंधित देखें

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

एक नया उदाहरण प्रारंभ करता है [`PrimaveraXmlReader`](../) क्लास का।

```csharp
public PrimaveraXmlReader(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | Primavera Xml सामग्री युक्त स्ट्रीम। |

## उदाहरण

दिखाता है कि Primavera XML स्ट्रीम से प्रोजेक्ट कैसे आयात करें।

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### संबंधित देखें

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


