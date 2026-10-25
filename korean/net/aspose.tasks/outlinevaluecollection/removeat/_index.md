---
title: "OutlineValueCollection.RemoveAt"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineValueCollection 메서드. 지정된 인덱스에서 항목을 제거합니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks/outlinevaluecollection/removeat/
---
## OutlineValueCollection.RemoveAt method

지정된 인덱스의 항목을 제거합니다.

```csharp
public void RemoveAt(int index)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 인덱스 | Int32 | 항목을 제거할 지정된 0 기반 인덱스. |

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

* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


