---
title: "MpdSettings.MpdSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ MpdSettings. يهيئ مثيلاً جديداً من فئة MpdSettings"
type: docs
weight: 10
url: /ar/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

يهيئ مثيلاً جديداً من فئة [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| connectionString | سلسلة | سلسلة الاتصال المحددة. |
| projectId | Int32 | المعرف المحدد لمشروع للقراءة. |

## الأمثلة

يوضح كيفية قراءة مشروع من ملف MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


