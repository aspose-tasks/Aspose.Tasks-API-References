---
title: "클래스 OutlineValueCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineValueCollection 클래스. OutlineValue 객체의 컬렉션을 나타냅니다."
type: docs
weight: 1220
url: /ko/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

[`OutlineValue`](../outlinevalue/) 객체의 컬렉션을 나타냅니다.

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |

## 예제

개요 값 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 값 컬렉션 지우기
foreach (var outlineCode in project.OutlineCodes)
{
    // 개요 마스크 지우기
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// 인덱스 접근으로 값 업데이트
codeDefinition.Values[0].Value = "654321";

// 개요 값을 반복합니다
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// 개요 값 작업
// ...

// 필요할 때 값을 제거합니다
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// 시작 위치에 값을 삽입합니다
codeDefinition.Values.Insert(0, value);

// 삽입된 값의 위치를 확인합니다
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// 개요 값 작업
// ...

// 컬렉션에서 마지막 값을 제거합니다
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// 다른 개요 코드 정의를 만들 수 있습니다
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// 그런 다음 개요 값을 복사합니다
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### 또 보기

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


