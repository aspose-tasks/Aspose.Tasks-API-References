---
title: "Rsc.NotesText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. نص الملاحظات العادي المستخرج من بيانات RTF"
type: docs
weight: 480
url: /ar/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

النص العادي للملاحظات المستخرج من بيانات RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


