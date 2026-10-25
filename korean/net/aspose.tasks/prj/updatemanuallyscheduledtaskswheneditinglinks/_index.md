---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 링크가 편집될 때 수동 작업을 업데이트해야 하는지 여부를 결정합니다"
type: docs
weight: 770
url: /ko/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

링크가 편집될 때 수동 작업을 업데이트해야 하는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## 예제

Prj.UpdateManuallyScheduledTasksWhenEditingLinks 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


