---
title: "Rsc.NotesText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. RTF verilerinden çıkarılan notların düz metni."
type: docs
weight: 480
url: /tr/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

RTF verilerinden çıkarılan notların düz metni.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Örnekler

Rsc.NotesText özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


