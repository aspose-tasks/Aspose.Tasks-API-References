---
title: "ResourceAssignment.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. ResourceAssignment sınıfının örneği için bir karma kod değeri döndürür"
type: docs
weight: 710
url: /tr/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

[`ResourceAssignment`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir kaynak atamasının karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// atanmanın karma kodlarını yazdır
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


