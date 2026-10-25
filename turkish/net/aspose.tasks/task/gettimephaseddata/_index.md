---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Belirtilen zaman aşamalı veri tipinin verilen başlangıç ve bitiş tarihleri arasındaki TimephasedData değerlerini içeren TimephasedDataCollection nesnesini döndürür."
type: docs
weight: 1360
url: /tr/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Belirtilen zaman aşamalı veri tipinin verilen başlangıç ve bitiş tarihleri arasındaki [`TimephasedData`](../timephaseddata/) değerlerini içeren [`TimephasedDataCollection`](../../timephaseddatacollection/) nesnesini döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |
| timephasedType | TimephasedDataType | Zaman aşamalı veri türü ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Dönüş Değeri

Belirtilen zaman aşamalı veri tipinin verilen başlangıç ve bitiş tarihleri arasındaki [`TimephasedData`](../timephaseddata/) değerlerini içeren bir [`TimephasedDataCollection`](../../timephaseddatacollection/) nesnesi.

## Örnekler

Görevin zaman aşamalı verisini (belirli bir tip ile) nasıl alacağınızı gösterir.

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

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Verilen başlangıç ve bitiş tarihleri arasındaki [`TimephasedData`](../timephaseddata/) değerlerini içeren [`TimephasedDataCollection`](../../timephaseddatacollection/) nesnesini döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |

### Dönüş Değeri

Doldurulacak [`TimephasedData`](../../timephaseddata/) listesi.

## Örnekler

Görev için zaman aşamalı verileri (TaskWork türüyle) nasıl alacağınızı gösterir.

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

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


