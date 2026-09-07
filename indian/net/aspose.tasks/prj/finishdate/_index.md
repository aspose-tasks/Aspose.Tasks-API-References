---
title: "Prj.FinishDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj field. एक परियोजना की समाप्ति तिथि"
type: docs
weight: 330
url: /hi/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

परियोजना की समाप्ति तिथि।

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को प्रारंभ तिथि के बजाय समाप्ति तिथि से कैसे पुनः‑शेड्यूल किया जाए।

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// अब सभी कार्यों की तिथियाँ (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) गणना की गई हैं। क्रिटिकल पाथ प्राप्त करने के लिए हमें स्लैक की गणना करनी होगी (इसे अलग थ्रेड में बुलाया जा सकता है, लेकिन सभी प्रारंभ/समाप्ति तिथियों की गणना के बाद ही)।
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


