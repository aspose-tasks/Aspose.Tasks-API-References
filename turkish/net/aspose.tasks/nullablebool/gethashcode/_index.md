---
title: "NullableBool.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yöntemi. NullableBool sınıfının örneği için bir karma kod değeri döndürür"
type: docs
weight: 50
url: /tr/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

[`NullableBool`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

&lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode yönteminin nasıl kullanılacağını gösterir.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool'ların karma kodu 'IsDefined' ve 'Value' özelliklerine dayanır
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Ayrıca Bakınız

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


