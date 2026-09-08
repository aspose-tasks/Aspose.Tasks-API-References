---
title: "클래스 EntityFieldAttribute"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute 클래스. 엔터티 속성을 위한 특성을 나타냅니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

엔터티 속성을 위한 특성을 나타냅니다.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | 기본 생성자입니다. |

## 비고

[`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) 및 [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) 엔터티 속성에만 사용되는 특성이며, 열거를 단순화합니다.

## 예제

**EntityField** 특성을 사용하여 속성을 열거하는 방법:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### 또 보기

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


