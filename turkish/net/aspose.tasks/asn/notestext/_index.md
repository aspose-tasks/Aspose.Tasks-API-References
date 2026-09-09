---
title: "Asn.NotesText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. RTF verisinden çıkarılan notların düz metni"
type: docs
weight: 350
url: /tr/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

RTF verilerinden çıkarılan notların düz metni.

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


