---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraXerReader कंस्ट्रक्टर। PrimaveraXerReader क्लास का एक नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

[`PrimaveraXerReader`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| xerFilePath | स्ट्रिंग | .xer फ़ाइल का पथ जहाँ Primavera परियोजना या परियोजनाएँ स्थित हैं। |

## उदाहरण

दिखाता है कि Primavera XER फ़ाइल से छोटे प्रोजेक्ट्स की जानकारी कैसे जांचें।

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### संबंधित देखें

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

[`PrimaveraXerReader`](../) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public PrimaveraXerReader(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | Primavera XER सामग्री वाला स्ट्रीम। |

### संबंधित देखें

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


