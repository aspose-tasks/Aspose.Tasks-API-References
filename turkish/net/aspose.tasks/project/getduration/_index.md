---
title: "Project.GetDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Belirtilen birim sayısı ve proje ayarlarında tanımlı varsayılan süre formatı ile Duration nesnesini alır."
type: docs
weight: 1100
url: /tr/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Belirtilen birim sayısı ve projenin ayarlarında tanımlı varsayılan süre formatı ile [`Duration`](../../duration/) nesnesini alır [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Double | belirtilen birim sayısı. |

### Dönüş Değeri

Duration nesnesi.

## Açıklamalar

Bu yöntem dikkatli kullanılmalıdır çünkü Project.DurationFormat ayarına bağlı olarak farklı süreler döndürür. Örneğin, GetWork(1.0) Project.DurationFormat TimeUnitType.Hour olduğunda 1 saat, Project.DurationFormat TimeUnitType.Day olduğunda 1 gün döndürür.

## Örnekler

Proje fabric yöntemlerini kullanarak varsayılan projenin süre formatı ile bir &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; örneği nasıl oluşturacağınızı gösterir.

```csharp
var project = new Project();

// varsayılan proje formatı ile bir süre alın.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Belirtilen [`TimeUnitType`](../../timeunittype/) birim sayısı ile [`Duration`](../../duration/) nesnesini alır.

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Double | belirtilen birim sayısı. |
| timeUnit | TimeUnitType | belirtilen TimeUnitType değeri. |

### Dönüş Değeri

Duration nesnesi.

## Örnekler

Proje fabric yöntemlerini kullanarak bir &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; örneği nasıl oluşturacağınızı gösterir.

```csharp
var project = new Project();

// varsayılan proje formatı ile bir süre alın.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Belirtilen TimeSpan değeri ve belirtilen [`TimeUnitType`](../../timeunittype/) değeri ile [`Duration`](../../duration/) nesnesini alır.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| timeSpan | TimeSpan | belirtilen TimeSpan değeri. |
| timeUnit | TimeUnitType | belirtilen TimeUnitType değeri. |

### Dönüş Değeri

Duration nesnesi.

### Ayrıca Bakınız

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


