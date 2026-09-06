---
title: "Resource.GetTimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تُرجع نسخة من الفئة TimephasedDataCollection لهذا الكائن مع قيم TimephasedData ضمن تواريخ البدء والنهاية المحددة لنوع TimephasedDataType المحدد"
type: docs
weight: 850
url: /ar/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

تُرجع نسخة من الفئة [`TimephasedDataCollection`](../../timephaseddatacollection/) لهذا الكائن مع قيم [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة لنوع [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للبيانات المرحلية. |
| نهاية | DateTime | تاريخ النهاية للبيانات المرحلية. |
| timephasedType | TimephasedDataType | نوع البيانات المرحلية ([`TimephasedDataType`](../../timephaseddatatype/)). |

### قيمة الإرجاع

قائمة بـ [`TimephasedData`](../timephaseddata/).

## الأمثلة

يوضح كيفية قراءة البيانات المرحلية للموارد الخاصة بالعمل/التكلفة.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// احصل على Resource باستخدام معرّفه
var resource = project.Resources.GetByUid(1);

// اطبع البيانات المرحلية لـ ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// اطبع البيانات المرحلية لـ ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

تُرجع [`TimephasedDataCollection`](../../timephaseddatacollection/) لهذا الكائن مع قيم [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للبيانات المرحلية. |
| نهاية | DateTime | تاريخ النهاية للبيانات المرحلية. |

### قيمة الإرجاع

قائمة بـ [`TimephasedData`](../../timephaseddata/).

## الأمثلة

يوضح كيفية قراءة البيانات المرحلية للموارد الخاصة بالعمل/التكلفة.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// احصل على Resource باستخدام معرّفه
var resource = project.Resources.GetByUid(1);

// اطبع البيانات المرحلية لـ ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// اطبع البيانات المرحلية لـ ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


