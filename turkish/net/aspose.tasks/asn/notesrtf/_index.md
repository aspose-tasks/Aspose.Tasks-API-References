---
title: "Asn.NotesRTF"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. RTF formatındaki metin notları. Yalnızca MPP formatları için desteklenir"
type: docs
weight: 340
url: /tr/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

RTF formatındaki metin notları. Yalnızca MPP formatları için desteklenir.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## Örnekler

Kaynak atama notlarını almayı/ayarlamayı gösterir.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// kaynak ataması oluştur
var assn = project.ResourceAssignments.Add(task, rsc);

// kaynak atama notlarını ayarla 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


