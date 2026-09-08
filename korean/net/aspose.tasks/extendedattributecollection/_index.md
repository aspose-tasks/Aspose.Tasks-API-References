---
title: "클래스 ExtendedAttributeCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ExtendedAttributeCollection 클래스. ExtendedAttribute 객체의 컬렉션을 나타냅니다"
type: docs
weight: 530
url: /ko/net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

[`ExtendedAttribute`](../extendedattribute/) 객체의 컬렉션을 나타냅니다.

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | 지정된 인덱스의 요소를 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |

## 예제

확장 속성 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 인덱스 0인 작업을 가져옵니다
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // 확장 속성을 지웁니다
    task.ExtendedAttributes.Clear();
}

// 작업에 대한 확장 속성 정의를 생성합니다
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// 확장 속성 1을 추가합니다
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// 확장 속성 2를 추가합니다
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// 확장 속성을 사용합니다...

// 인덱스로 확장 속성을 제거합니다
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// 컬렉션 인덱스 접근을 사용합니다
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// 속성을 다른 프로젝트에 복사합니다
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// 모든 확장 속성 정의를 제거합니다
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### 또 보기

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


