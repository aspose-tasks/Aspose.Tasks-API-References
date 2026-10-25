---
title: "클래스 OutlineCodeCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineCodeCollection 클래스. OutlineCode 객체의 컬렉션을 나타냅니다."
type: docs
weight: 1160
url: /ko/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

[`OutlineCode`](../outlinecode/) 객체의 컬렉션을 나타냅니다.

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |

## 예제

아웃라인 코드 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// 사용자 지정 아웃라인 코드 정의를 추가합니다.
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// 아웃라인 코드를 생성합니다.
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// 컬렉션이 읽기 전용이 아님을 확인할 수 있습니다.
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// 잘못된 위치에 2와 함께 코드를 삽입합니다.
task.OutlineCodes.Insert(0, code2);

// 수정합니다.
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// 올바른 위치에 2와 함께 코드를 삽입합니다.
task.OutlineCodes.Insert(2, code2);

// 코드가 삽입되었는지 확인합니다.
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// 아웃라인 코드를 작업합니다.
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// 사용자 지정 아웃라인 코드 정의를 추가합니다.
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// 아웃라인 코드를 생성합니다.
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// 아웃라인 코드를 작업합니다.
// ...

// 아웃라인 코드를 제거합니다.
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// 한 번에 모든 값을 지웁니다.
task.OutlineCodes.Clear();
```

### 또 보기

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


