---
title: "Resource.Set"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler"
type: docs
weight: 860
url: /tr/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| Parametre | Açıklama |
| --- | --- |
| T | eşlenen değerin tipi. |
| key | belirtilen özellik anahtarı. [`Rsc`](../../rsc/) özellik anahtarını almak için. |
| val | değer. |

## Örnekler

Ortak kaynak özelliklerinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Kaynak ekle ve bazı özellikleri ayarla
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

Belirtilen özelliği bu kapsayıcıda belirtilen değere eşler.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | Key`2 | belirtilen özellik anahtarı. [`Rsc`](../../rsc/) özellik anahtarını almak için. |
| val | DateTime | değer. |

## Örnekler

Ortak kaynak özelliklerinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Kaynak ekle ve bazı özellikleri ayarla
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


