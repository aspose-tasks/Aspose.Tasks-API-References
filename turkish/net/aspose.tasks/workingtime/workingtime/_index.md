---
title: WorkingTime.WorkingTime
second_title: Aspose.Tasks for .NET API Referansı
description: WorkingTime inşaatçı. Yeni bir örneğini başlatır.WorkingTime belirtilen başlangıç ve bitiş saatlerine sahip bir aralığa sahip sınıf.
type: docs
weight: 10
url: /tr/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Yeni bir örneğini başlatır.[`WorkingTime`](../) belirtilen başlangıç ve bitiş saatlerine sahip bir aralığa sahip sınıf.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fromTime | DateTime | aralık başlangıç zamanı |
| toTime | DateTime | aralık bitiş zamanı |

### Ayrıca bakınız

* class [WorkingTime](../)
* ad alanı [Aspose.Tasks](../../workingtime/)
* toplantı [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Yeni bir örneğini başlatır.[`WorkingTime`](../) belirtilen başlangıç ve bitiş zamanlarına sahip bir aralık öğesi içeren sınıf.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fromTime | TimeSpan | Aralık başlangıç zamanı ile temsil edilirTimeSpan yapı |
| toTime | TimeSpan | Aralığın bitiş zamanı şununla temsil edilir:TimeSpan yapı |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | toTime, toTime argümanına değerinden küçük olduğunda veya fromTime ile toTime arasındaki aralık 24 saatten fazla olduğunda. |

### Örnekler

WorkingTime ctor'ın aşırı yüklemesi, TimeSpans: kullanılarak aralığın başlangıcını ve bitişini başlatmak için kullanılabilir.

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Ayrıca bakınız

* class [WorkingTime](../)
* ad alanı [Aspose.Tasks](../../workingtime/)
* toplantı [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Yeni bir örneğini başlatır.[`WorkingTime`](../) belirtilen başlangıç ve bitiş zamanlarına sahip bir aralık öğesi içeren sınıf.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fromHours | Int32 | Aralığın başlangıç zamanı, saatlerin tam sayısıyla temsil edilir (0-24). |
| toHours | Int32 | Aralığın bitiş zamanı, saatlerin tam sayısıyla temsil edilir (0-24). |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentException | toTime, toTime argümanına değerinden küçük olduğunda veya fromTime ile toTime arasındaki aralık 24 saatten fazla olduğunda. |

### Örnekler

WorkingTime ctor'ın aşırı yüklemesi, tam saat: kullanılarak aralığın başlangıç ve bitişini başlatmak için kullanılabilir.

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### Ayrıca bakınız

* class [WorkingTime](../)
* ad alanı [Aspose.Tasks](../../workingtime/)
* toplantı [Aspose.Tasks](../../../)


