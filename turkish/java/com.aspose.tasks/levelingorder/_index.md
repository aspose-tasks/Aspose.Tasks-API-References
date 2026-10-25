---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Dengeleme sırasının olası değerlerini tanımlar."
type: docs
weight: 143
url: /tr/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Dengeleme sırasının olası değerlerini tanımlar.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [IdOnly](#IdOnly) | Görevler Id artan sırasına göre geciktirilir. |
| [PriorityThenStandard](#PriorityThenStandard) | Öncelik ilk olarak dikkate alınır, ardından Standard'daki aynı özellikler. |
| [Standard](#Standard) | Aşağıdaki özellikler dikkate alınır: önceki görev ilişkileri, toplam gecikme (daha yüksek toplam gecikmeye sahip görev önce geciktirilir), başlangıç tarihi, öncelik. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Görevler Id artan sırasına göre geciktirilir.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


Öncelik ilk olarak dikkate alınır, ardından Standard'daki aynı özellikler.

### Standard {#Standard}
```
public static final int Standard
```


Aşağıdaki özellikler dikkate alınır: önceki görev ilişkileri, toplam gecikme (daha yüksek toplam gecikmeye sahip görev önce geciktirilir), başlangıç tarihi, öncelik. Bu varsayılan değerdir.

