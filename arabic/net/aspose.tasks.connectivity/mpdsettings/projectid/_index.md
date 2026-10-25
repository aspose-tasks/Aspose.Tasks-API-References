---
title: "MpdSettings.ProjectId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MpdSettings. تحصل على معرف المشروع للقراءة"
type: docs
weight: 20
url: /ar/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

يحصل على معرف المشروع المراد قراءته.

```csharp
public int ProjectId { get; }
```

## الأمثلة

يوضح كيفية استخدام إعدادات MPD للتحكم في استيراد المشروع من قاعدة البيانات.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


