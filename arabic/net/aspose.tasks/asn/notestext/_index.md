---
title: "Asn.NotesText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. نص الملاحظات العادي المستخرج من بيانات RTF"
type: docs
weight: 350
url: /ar/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

النص العادي للملاحظات المستخرج من بيانات RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
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


