---
title: TaskCollection.Add
second_title: Aspose.Tasks for .NET API Referansı
description: TaskCollection yöntem. Belirtilen görevi örneğine ekleyin.TaskCollectionclass. Eğer ParentProject.CalculationMode Yok ise kullanıcı bu yöntemi kullandıktan sonra Project.Recalculatei çağırmalıdır Tüm proje görevlerini yeniden planlar başlangıç/bitiş tarihleri erken/geç tarihleri ayarlar ve bolluklar iş gibi bağımlı alanları hesaplar ve maliyet alanları kimlikler ve anahat seviyeleri. ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini anahat seviyesini ve anahat numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Otomatik ise yöntem tüm projenin görevlerini otomatik olarak yeniden planlar başlangıç/bitiş tarihler erken/geç tarihleri ayarlar bollukları çalışma ve maliyet alanlarını hesaplar kimlikleri ve anahat düzeylerini yeniden hesaplar.
type: docs
weight: 50
url: /tr/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Belirtilen görevi örneğine ekleyin.[`TaskCollection`](../)class. Eğer ParentProject.CalculationMode Yok ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate()'i çağırmalıdır (Tüm proje görevlerini yeniden planlar (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar) ve bolluklar, iş gibi bağımlı alanları hesaplar) ve maliyet alanları, kimlikler ve anahat seviyeleri). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, anahat seviyesini ve anahat numaralarını otomatik olarak hesaplar. ParentProject.CalculationMode Otomatik ise, yöntem tüm projenin görevlerini otomatik olarak yeniden planlar (başlangıç/bitiş) tarihler, erken/geç tarihleri ayarlar, bollukları, çalışma ve maliyet alanlarını hesaplar, kimlikleri ve anahat düzeylerini yeniden hesaplar).

```csharp
public void Add(Task item)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| item | Task | bu görev koleksiyonuna eklenmesi gereken belirtilen görev. |

### Ayrıca bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* ad alanı [Aspose.Tasks](../../taskcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add() {#add}

Proje görevleri koleksiyonuna, son görevin aynı ana hat düzeyinde yeni görev ekler.

```csharp
public Task Add()
```

### Geri dönüş değeri

yeni eklenen örneğini döndürür[`Task`](../../task/) sınıf.

### Ayrıca bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* ad alanı [Aspose.Tasks](../../taskcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Alt görevler koleksiyonuna yeni bir görev ekler.

```csharp
public Task Add(string taskName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| taskName | String | belirtilen görev adı. |

### Geri dönüş değeri

yeni eklenen örneğini döndürür[`Task`](../../task/) sınıf.

### Ayrıca bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* ad alanı [Aspose.Tasks](../../taskcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Alt görev koleksiyonuna yeni bir yinelenen görev ekler.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| taskName | String | belirtilen görev adı. |
| beforeTaskId | Int32 | Önüne yeni bir görevin ekleneceği görevin belirtilen kimliği. |

### Geri dönüş değeri

belirtilen kimliğe sahip bir görevden önce eklenen bir görevi döndürür.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | Belirtilen kimlik geçerli bir görev kimliği değilse ArgumentOutOfRangeException atılır. |

### Ayrıca bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* ad alanı [Aspose.Tasks](../../taskcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Belirtilen kimliğe sahip ve aynı ana hat seviyesindeki bir görevin önüne yeni bir görev ekler.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Parametreler, yinelenen görevin oluşturulması için belirtilen parametrelerdir. |

### Geri dönüş değeri

yeni eklenen örneğini döndürür[`Task`](../../task/) sınıf.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Belirtilen parametreler boşsa atılır. |
| ArgumentException | Belirtilen parametreler geçersizse atılır. |

### Ayrıca bakınız

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* ad alanı [Aspose.Tasks](../../taskcollection/)
* toplantı [Aspose.Tasks](../../../)


