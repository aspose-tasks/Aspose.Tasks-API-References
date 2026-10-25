---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Resource sınıfının örneği için bir hash kodu değeri döndürür"
type: docs
weight: 840
url: /tr/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

[`Resource`](../) sınıfının örneği için bir hash kodu değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir kaynağın hash kodunun nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// bir kaynağın hash kodu resource UID'ye eşittir
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


