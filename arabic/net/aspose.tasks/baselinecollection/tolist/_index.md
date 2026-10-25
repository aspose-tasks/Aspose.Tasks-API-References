---
title: "BaselineCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة BaselineCollection. تُحوّل كائن BaselineCollection إلى قائمة من كائنات Baseline"
type: docs
weight: 70
url: /ar/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

يحوِّل كائن BaselineCollection إلى قائمة من كائنات [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### قيمة الإرجاع

قائمة من كائنات [`Baseline`](../../baseline/).

## الأمثلة

يوضح كيفية العمل مع مجموعات Baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// قراءة معلومات الخط الأساسي
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### انظر أيضًا

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


