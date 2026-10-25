---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API-referens"
description: "Definierar de möjliga värdena för nivåordning."
type: docs
weight: 143
url: /sv/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Definierar de möjliga värdena för nivåordning.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [IdOnly](#IdOnly) | Uppgifter försenas i stigande Id‑ordning. |
| [PriorityThenStandard](#PriorityThenStandard) | Prioriteten beaktas först, sedan samma egenskaper som i Standard. |
| [Standard](#Standard) | Följande egenskaper beaktas: föregångarrelationer, total marginal (en uppgift med högre total marginal försenas först), startdatum, prioritet. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Uppgifter försenas i stigande Id‑ordning.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


Prioriteten beaktas först, sedan samma egenskaper som i Standard.

### Standard {#Standard}
```
public static final int Standard
```


Följande egenskaper beaktas: föregångarrelationer, total marginal (en uppgift med högre total marginal försenas först), startdatum, prioritet. Detta är standardvärdet.

