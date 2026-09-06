---
title: "BuiltInProjectPropertyCollection.IsReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "BuiltInProjectPropertyCollection خاصية. يحصل على قيمة تشير إلى ما إذا كان هذا التجميع للقراءة فقط أم لا false"
type: docs
weight: 60
url: /ar/net/aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/
---
## BuiltInProjectPropertyCollection.IsReadOnly property

يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

```csharp
public override bool IsReadOnly { get; }
```

## الأمثلة

يوضح كيفية قراءة خصائص المشروع المدمجة.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// التكرار على مجموعة الخصائص المدمجة
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### انظر أيضًا

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


