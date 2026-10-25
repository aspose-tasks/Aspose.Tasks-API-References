---
title: "Rsc.OvertimeRate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak tarafından yapılan fazla mesai çalışması için ödeme oranı"
type: docs
weight: 510
url: /tr/net/aspose.tasks/rsc/overtimerate/
---
## Rsc.OvertimeRate field

Kaynağın yaptığı fazla mesai çalışması için ödeme oranı.

```csharp
public static readonly Key<decimal, RscKey> OvertimeRate;
```

## Örnekler

Kaynak oranları ve gruplarıyla nasıl çalışılacağını gösterir.

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
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


