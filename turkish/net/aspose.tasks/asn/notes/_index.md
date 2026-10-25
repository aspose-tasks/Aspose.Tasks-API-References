---
title: "Notlar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Bir atama ile ilişkili metin notları."
type: docs
weight: 350
url: /tr/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

Bir atama ile ilişkili metin notları.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### Örnekler

Kaynak atama notlarını almayı/ayarlamayı gösterir.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// kaynak ataması oluştur
var assn = project.ResourceAssignments.Add(task, rsc);

// kaynak atama notlarını ayarla 
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- DÜZENLEMEYİN: xmldocmd tarafından Aspose.Tasks.dll için oluşturuldu -->
