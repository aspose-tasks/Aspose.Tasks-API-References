---
title: "NullableBool.NullableBool"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yapıcı. Belirtilen boolean değerle NullableBool yapısının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Belirtilen boolean değerle [`NullableBool`](../) yapısının yeni bir örneğini başlatır.

```csharp
public NullableBool(bool value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | Boolean | belirtilen boolean değeri. |

## Örnekler

&lt;see cref=\"NullableBool\" /&gt; sınıfı ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının nerede kullanıldığını kontrol edelim
// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının temel avantajı
// Birisi, oluşturma yoluyla onu tanımsız olarak ayarlayabilir
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// nullable bool örneğini kullan
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// nullable bool örneğini kullan
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Ayrıca Bakınız

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## NullableBool(bool, bool) {#constructor_1}

Yeni bir [`NullableBool`](../) yapısının örneğini başlatır.

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | Boolean | Geçerli değer. |
| isDefined | Boolean | Geçerli değerin tanımlı olup olmadığını gösteren değer. |

## Örnekler

&lt;see cref=\"NullableBool\" /&gt; sınıfı ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının nerede kullanıldığını kontrol edelim
// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının temel avantajı
// Birisi, oluşturma yoluyla onu tanımsız olarak ayarlayabilir
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// nullable bool örneğini kullan
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// nullable bool örneğini kullan
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Ayrıca Bakınız

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


