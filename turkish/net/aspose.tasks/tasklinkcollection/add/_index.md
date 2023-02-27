---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks for .NET API Referansı
description: TaskLinkCollection yöntem. FinishStart örneğini döndürürTaskLink TaskLinkCollection nesnesine eklendi.
type: docs
weight: 40
url: /tr/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Finish-Start örneğini döndürür[`TaskLink`](../../tasklink/) TaskLinkCollection nesnesine eklendi.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pred | Task | Önceki görev. |
| succ | Task | Ardıl görev. |

### Geri dönüş değeri

bu nesneye eklenmiş bir görev bağlantısı örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Giriş görevlerinden herhangi biri null değerine eşitse, o zamanArgumentNullException atılacak. |

### Ayrıca bakınız

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* ad alanı [Aspose.Tasks](../../tasklinkcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

örneğini döndürür[`TaskLink`](../../tasklink/) TaskLinkCollection nesnesine eklendi.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pred | Task | Önceki görev. |
| succ | Task | Ardıl görev. |
| linkType | TaskLinkType | Bağlantı türü[`TaskLinkType`](../../tasklinktype/) |

### Geri dönüş değeri

bu nesneye eklenmiş bir görev bağlantısı örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Giriş görevlerinden herhangi biri null değerine eşitse, o zamanArgumentNullException atılacak. |

### Ayrıca bakınız

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* ad alanı [Aspose.Tasks](../../tasklinkcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

örneğini döndürür[`TaskLink`](../../tasklink/) TaskLinkCollection nesnesine eklendi.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pred | Task | Önceki görev. |
| succ | Task | Ardıl görev. |
| linkType | TaskLinkType | Bağlantı türü[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Bağlantı gecikmesi[`Duration`](../../duration/). |

### Geri dönüş değeri

bu nesneye eklenmiş bir görev bağlantısı.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Giriş görevlerinden herhangi biri null değerine eşitse, o zamanArgumentNullException atılacak. |

### Ayrıca bakınız

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* ad alanı [Aspose.Tasks](../../tasklinkcollection/)
* toplantı [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Bu, ICollection'ın Add yönteminin saplama uygulamasıdır ve yalnızca NotSupportedException öğesini atar.

```csharp
public void Add(TaskLink item)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| item | TaskLink | Eklenecek öğe. |

### Ayrıca bakınız

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* ad alanı [Aspose.Tasks](../../tasklinkcollection/)
* toplantı [Aspose.Tasks](../../../)


