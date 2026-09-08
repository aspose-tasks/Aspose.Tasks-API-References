---
title: "OutlineCodeCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineCodeCollection 속성. 이 컬렉션에 포함된 요소 수를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/outlinecodecollection/count/
---
## OutlineCodeCollection.Count property

이 컬렉션에 포함된 요소 수를 가져옵니다.

```csharp
public int Count { get; }
```

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

* class [OutlineCodeCollection](../)
* namespace [Aspose.Tasks](../../outlinecodecollection/)
* assembly [Aspose.Tasks](../../../)


