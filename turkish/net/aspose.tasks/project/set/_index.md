---
title: "Project.Set"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Belirtilen özelliği bu konteynerde belirtilen değere eşler"
type: docs
weight: 1240
url: /tr/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parametre | Açıklama |
| --- | --- |
| T | eşlenen değerin tipi. |
| key | belirtilen özellik anahtarı. Özellik anahtarını almak için [`Prj`](../../prj/). |
| val | değer. |

## Örnekler

Görev niteliklerinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | Key`2 | belirtilen özellik anahtarı. Özellik anahtarını almak için [`Prj`](../../prj/). |
| val | DateTime | değer. |

## Örnekler

Görev niteliklerinin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


