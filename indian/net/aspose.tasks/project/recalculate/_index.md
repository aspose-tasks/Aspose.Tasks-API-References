---
title: "Project.Recalculate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। सभी प्रोजेक्ट टास्क आईडी, आउटलाइन लेवल, प्रारंभ/समाप्ति तिथियों को पुनः शेड्यूल करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड्स की गणना करता है"
type: docs
weight: 1150
url: /hi/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

सभी परियोजना टास्क आईडी, रूपरेखा स्तर, प्रारंभ/समाप्ति तिथियों को पुनर्निर्धारित करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है।

```csharp
public void Recalculate()
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को समाप्ति तिथि के बजाय प्रारंभ तिथि से कैसे पुनर्निर्धारित किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// अब सभी कार्यों की तिथियाँ (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) गणना की गई हैं। क्रिटिकल पाथ प्राप्त करने के लिए हमें स्लैक की गणना करनी होगी (इसे अलग थ्रेड में बुलाया जा सकता है, लेकिन सभी प्रारंभ/समाप्ति तिथियों की गणना के बाद ही)।
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

वैकल्पिक सत्यापन के साथ सभी परियोजना टास्क आईडी, रूपरेखा स्तर, प्रारंभ/समाप्ति तिथियों को पुनर्निर्धारित करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है।

```csharp
public void Recalculate(bool validate)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| validate | Boolean | यदि true हो तो पुनर्गणना की वैधता लागू की जाएगी। कौन सा डेटा मान्य किया जाता है: वर्तमान में केवल कार्य और कार्य लिंक तिथि रेंज की बुनियादी वैधता लागू है। कार्य की तिथि रेंज (जैसे ActualStart - ActualFinish, EarlyStart - EarlyFinish, आदि) तथा कार्य लिंक तिथियों की जाँच इस मानदंड के विरुद्ध की जाएगी कि प्रारंभ तिथि समाप्ति तिथि से कम या बराबर हो। यदि ऊपर वर्णित किसी भी शर्त में विफलता होती है तो [`RecalculationValidationException`](../../recalculationvalidationexception/) फेंका जाएगा। |

## उदाहरण

दिखाता है कि पोस्ट वैधता के साथ प्रोजेक्ट को कैसे पुनः गणना किया जाए।

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // पोस्ट वैधता के साथ प्रोजेक्ट को पुनः गणना करें
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


