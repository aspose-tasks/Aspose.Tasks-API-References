---
title: "Task.GetTimephasedData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُرجع كائن TimephasedDataCollection مع قيم TimephasedData ضمن تواريخ البدء والنهاية المحددة لنوع البيانات الزمنية المحدد."
type: docs
weight: 1360
url: /ar/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

يرجع كائن [`TimephasedDataCollection`](../../timephaseddatacollection/) مع قيم [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة لنوع البيانات الزمنية المحدد.

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

كائن [`TimephasedDataCollection`](../../timephaseddatacollection/) مع قيم [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة لنوع البيانات الزمنية المحدد.

## الأمثلة

يعرض كيفية الحصول على بيانات زمنية (بنمط محدد) للمهمة.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

يرجع كائن [`TimephasedDataCollection`](../../timephaseddatacollection/) مع قيم [`TimephasedData`](../timephaseddata/) ضمن تواريخ البدء والنهاية المحددة.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للبيانات المرحلية. |
| نهاية | DateTime | تاريخ النهاية للبيانات المرحلية. |

### قيمة الإرجاع

قائمة بـ [`TimephasedData`](../../timephaseddata/) لتعبئتها.

## الأمثلة

يوضح كيفية الحصول على بيانات زمنية (مع نوع TaskWork) للمهمة.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### انظر أيضًا

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


