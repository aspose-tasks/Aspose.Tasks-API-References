---
title: "Rsc.Group"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 속한 그룹"
type: docs
weight: 300
url: /ko/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

리소스가 속한 그룹입니다.

```csharp
public static readonly Key<string, RscKey> Group;
```

## 예제

리소스 요율 및 그룹을 다루는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// 리소스를 추가하고 일부 속성을 설정합니다
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

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


