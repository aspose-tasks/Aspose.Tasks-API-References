---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि प्रोजेक्ट शेड्यूल को प्रारंभ तिथि से आगे की गणना करनी है या नहीं"
type: docs
weight: 630
url: /hi/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

निर्धारित करता है कि क्या प्रारंभ तिथि से परियोजना शेड्यूल को आगे की ओर गणना किया जाए।

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


