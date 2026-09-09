---
title: "NullableBool.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yöntemi. Geçerli nesneyi temsil eden bir dize döndürür."
type: docs
weight: 60
url: /tr/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Geçerli nesneyi temsil eden bir dize döndürür.

```csharp
public override string ToString()
```

### Dönüş Değeri

Geçerli nesneyi temsil eden bir dize.

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


