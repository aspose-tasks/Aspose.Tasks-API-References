---
title: "الفئة CompoundDocumentHeaderException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.CompoundDocumentHeaderException. تمثل استثناءً يُرمى عندما يكون رأس ملف MPP معطلاً."
type: docs
weight: 280
url: /ar/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

يمثل استثناء يُرمى عندما يكون رأس ملف MPP معطلاً.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## الأمثلة

يظهر كيفية التقاط استثناء &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

```csharp
try
{
    var project = new Project(DataDir + "Project1.mpp");

    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (CompoundDocumentHeaderException e)
{
    Console.WriteLine(e.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


