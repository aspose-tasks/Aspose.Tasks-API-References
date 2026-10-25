---
title: "क्लास VbaReferenceCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaReferenceCollection क्लास। VbaReference ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 2880
url: /hi/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

[`VbaReference`](../vbareference/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## उदाहरण

दिखाता है कि VBA रेफ़रेंस संग्रह के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### संबंधित देखें

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


