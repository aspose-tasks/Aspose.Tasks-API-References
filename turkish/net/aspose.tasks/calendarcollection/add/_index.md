---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. Bu CalendarCollection nesnesine yeni bir temel takvim ekler ve eklenen takvimi döndürür."
type: docs
weight: 20
url: /tr/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Bu CalendarCollection nesnesine yeni bir temel takvim ekler ve eklenen takvimi döndürür.

```csharp
public Calendar Add(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Takvim adı. |

### Dönüş Değeri

Eklenen [`Calendar`](../../calendar/) nesnesi.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | Takvim adı null olduğunda fırlatılır. |

## Örnekler

Standart bir takvim nasıl oluşturulur gösterir.

```csharp
var project = new Project();

// Bir takvim tanımlayın ve onu standart yapın
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Bu CalendarCollection nesnesine belirtilen temel takvimle yeni bir takvim ekler ve eklenen takvimi döndürür.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Belirtilen ad. |
| baseCalendar | Takvim | Belirtilen temel takvim. |

### Dönüş Değeri

Eklenen [`Calendar`](../../calendar/) nesnesi.

## Örnekler

Yeni takvimlerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project();

// Yeni takvimler, bir projenin takvim koleksiyonuna koleksiyonun Add aşırı yüklemeleri kullanılarak eklenebilir.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


