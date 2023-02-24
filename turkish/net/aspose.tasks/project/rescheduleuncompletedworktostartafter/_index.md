---
title: Project.RescheduleUncompletedWorkToStartAfter
second_title: Aspose.Tasks for .NET API Referansı
description: Project yöntem. Tamamlanmamış proje çalışmasını belirli bir tarihten sonra başlayacak şekilde yeniden planlar.
type: docs
weight: 1170
url: /tr/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

Tamamlanmamış proje çalışmasını belirli bir tarihten sonra başlayacak şekilde yeniden planlar.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| after | DateTime | Tamamlanmamış çalışmanın yeniden planlanacağı tarih. |

### Notlar

Bu yöntemi kullanmadan önce Project.CanSplitsInProgressTasks bayrağının true olarak ayarlandığından emin olun.

### Ayrıca bakınız

* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

Belirli bir görev listesi için tamamlanmamış işi belirtilen tarihten sonra başlayacak şekilde yeniden planlar.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| after | DateTime | Tamamlanmamış çalışmanın yeniden planlanacağı tarih. |
| taskCollection | List`1 | Tamamlanmamış işi yeniden planlamak için &lt;Görev&gt; görevlerini listele. |

### Notlar

Bu yöntemi kullanmadan önce Project.CanSplitsInProgressTasks bayrağının true olarak ayarlandığından emin olun.

### Ayrıca bakınız

* class [Task](../../task/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)


