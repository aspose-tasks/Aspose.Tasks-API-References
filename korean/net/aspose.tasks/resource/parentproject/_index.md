---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 이 컨테이너의 상위 프로젝트를 가져옵니다."
type: docs
weight: 600
url: /ko/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

이 컨테이너의 상위 프로젝트를 가져옵니다.

```csharp
public Project ParentProject { get; }
```

## 예제

리소스의 상위 프로젝트 사용 방법을 보여줍니다.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// 기본 프로젝트 작업 시간 단위 유형을 사용하여 리소스에 작업을 설정합니다.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### 또 보기

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


