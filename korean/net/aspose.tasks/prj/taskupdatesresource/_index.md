---
title: "Prj.TaskUpdatesResource"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 작업 업데이트가 리소스를 업데이트할지 여부를 결정합니다"
type: docs
weight: 710
url: /ko/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

작업에 대한 업데이트가 리소스를 업데이트하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## 예제

Prj.TaskUpdatesResource 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


