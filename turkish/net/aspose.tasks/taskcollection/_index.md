---
title: Class TaskCollection
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.TaskCollection sınıf. Bir koleksiyonu temsil ederTask nesneler.
type: docs
weight: 2100
url: /tr/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Bir koleksiyonu temsil eder[`Task`](../task/) nesneler.

```csharp
public class TaskCollection : IList<Task>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | TaskCollection. içinde bulunan nesnelerin sayısını alır. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Bu koleksiyonun salt okunur olup olmadığını gösteren bir değer alır. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Belirtilen dizindeki öğeyi döndürür. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | TaskCollection nesnesinin üst projesini alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Proje görevleri koleksiyonuna, son görevin aynı ana hat düzeyinde yeni görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Belirtilen kimliğe sahip ve aynı ana hat seviyesindeki bir görevin önüne yeni bir görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Alt görevler koleksiyonuna yeni bir görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Belirtilen görevi örneğine ekleyin.`TaskCollection`class. Eğer ParentProject.CalculationMode Yok ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate()'i çağırmalıdır (Tüm proje görevlerini yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) ve bolluklar, iş gibi bağımlı alanları hesaplar) ve maliyet alanları, kimlikler ve anahat seviyeleri). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, anahat seviyesini ve anahat numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Otomatik ise, yöntem tüm projenin görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş) tarihler, erken/geç tarihleri ayarlar, bollukları, çalışma ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Alt görev koleksiyonuna yeni bir yinelenen görev ekler. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Koleksiyonun belirtilen öğeyi içerip içermediğini kontrol eder. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Atası bu koleksiyonun üst görevi olan, belirtilen kimliğe sahip bir görev döndürür . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Atası bu koleksiyonun ana görevi olan, belirtilen Uid'ye sahip bir görev döndürür . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Bu koleksiyon için bir numaralandırıcı döndürür. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Bu, IList'in Insert yönteminin saplama uygulamasıdır ve yalnızca NotSupportedException öğesini atar. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Bu, ICollection'ın Remove yönteminin saplama uygulamasıdır ve yalnızca NotSupportedException öğesini atar. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | TaskCollection nesnesini bir listeye dönüştürür[`Task`](../task/) nesneler. |

### Ayrıca bakınız

* class [Task](../task/)
* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


