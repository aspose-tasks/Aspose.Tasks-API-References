---
title: "ExtendedAttributeCollection.Insert"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeCollection 메서드. 지정된 인덱스에 지정된 항목을 삽입합니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/extendedattributecollection/insert/
---
## ExtendedAttributeCollection.Insert method

지정된 인덱스에 지정된 항목을 삽입합니다.

```csharp
public void Insert(int index, ExtendedAttribute item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 인덱스 | Int32 | 항목을 삽입해야 하는 지정된 0 기반 인덱스. |
| 항목 | ExtendedAttribute | 이 컬렉션에 삽입할 지정된 항목. |

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


