---
title: "Asn.NotesRTF"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. ملاحظات النص بصيغة RTF. مدعومة لتنسيقات MPP فقط"
type: docs
weight: 340
url: /ar/net/aspose.tasks/asn/notesrtf/
---
## Asn.NotesRTF field

ملاحظات النص بتنسيق RTF. مدعومة فقط لتنسيقات MPP.

```csharp
public static readonly Key<string, AsnKey> NotesRTF;
```

## الأمثلة

يوضح كيفية الحصول على/تعيين ملاحظات تعيين الموارد.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// إنشاء تعيين مورد
var assn = project.ResourceAssignments.Add(task, rsc);

// تعيين ملاحظات تعيين الموارد 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


