---
title: "Rsc.Group"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. المجموعة التي ينتمي إليها المورد"
type: docs
weight: 300
url: /ar/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

المجموعة التي ينتمي إليها المورد.

```csharp
public static readonly Key<string, RscKey> Group;
```

## الأمثلة

يظهر كيفية التعامل مع معدلات الموارد والمجموعات.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// أضف موردًا واضبط بعض الخصائص
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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


