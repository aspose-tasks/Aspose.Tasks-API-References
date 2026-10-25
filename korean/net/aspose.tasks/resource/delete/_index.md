---
title: "Resource.Delete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "리소스 메서드. 프로젝트에서 리소스와 해당 할당을 삭제합니다"
type: docs
weight: 810
url: /ko/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

프로젝트에서 리소스와 해당 할당을 삭제합니다.

```csharp
public void Delete()
```

## 예제

리소스를 삭제하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// 리소스를 삭제합니다
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### 또 보기

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


