---
title: "Rsc.NotesRTF"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الملاحظات النصية بتنسيق RTF. مدعومة لتنسيقات MPP فقط"
type: docs
weight: 470
url: /ar/net/aspose.tasks/rsc/notesrtf/
---
## Rsc.NotesRTF field

ملاحظات النص بتنسيق RTF. مدعومة فقط لتنسيقات MPP.

```csharp
public static readonly Key<string, RscKey> NotesRTF;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.NotesRTF.

```csharp
var project = new Project();

            var resource = project.Resources.Add("Resource");

            const string RTF = @"{\rtf1\ansi\ansicpg1252\deff0\deflang1033{\fonttbl{\f0\fnil\fcharset134 SimSun;}{\f1\fnil\fcharset0 Calibri;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\sa200\sl276\slmult1\lang9\f0\fs22\'d4\'e7\'c9\'cf\'ba\'c3\f1\par
}
 "; // 早上好

            resource.Set(Rsc.NotesRTF, RTF);

            Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
            Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


