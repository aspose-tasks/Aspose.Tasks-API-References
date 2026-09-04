---
title: "Aspose::Tasks::WorkingTime::WorkingTime yapıcı"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "C++ için Aspose.Tasks"
description: "Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık içeren WorkingTime sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

Belirtilen başlangıç ve bitiş zamanlarıyla bir aralık içeren WorkingTime sınıfının yeni bir örneğini başlatır.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| Parametre | Açıklama |
| --- | --- |
| fromTime | aralık başlangıç zamanı |
| toTime | aralık bitiş zamanı |

---

## WorkingTime (2 of 3) {#workingtime_2}

WorkingTime sınıfının yeni bir örneğini, belirtilen başlangıç ve bitiş zamanlarına sahip bir aralık öğesiyle başlatır.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| Parametre | Açıklama |
| --- | --- |
| fromTime | Aralığın başlangıç zamanı, TimeSpan yapısı tarafından temsil edilir. |
| toTime | Aralığın bitiş zamanı, TimeSpan yapısı tarafından temsil edilir. |

---

## WorkingTime (3 of 3) {#workingtime_3}

WorkingTime sınıfının yeni bir örneğini, belirtilen başlangıç ve bitiş zamanlarına sahip bir aralık öğesiyle başlatır.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| Parametre | Açıklama |
| --- | --- |
| fromHours | Aralığın başlangıç zamanı, saat cinsinden tam sayı (0-24) ile temsil edilir. |
| toHours | Aralığın bitiş zamanı, saat cinsinden tam sayı (0-24) ile temsil edilir. |

