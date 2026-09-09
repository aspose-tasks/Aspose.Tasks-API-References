---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Proje kaynak atama listesinden geçersiz kaynak atamalarını ortadan kaldırır."
type: docs
weight: 1170
url: /tr/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Proje kaynak atamaları listesinden geçersiz kaynak atamalarını ortadan kaldırır.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Açıklamalar

MS Project her görev için boş bir kaynak ataması oluşturur. Bunları kaldırmak için yöntemi çağırın.

## Örnekler

Geçersiz atamaları nasıl kaldıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// geçersiz atamaları kaldır
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


