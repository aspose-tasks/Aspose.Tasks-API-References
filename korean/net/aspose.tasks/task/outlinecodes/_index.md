---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. OutlineCodeCollection 객체를 가져오거나 설정합니다"
type: docs
weight: 880
url: /ko/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

[`OutlineCodeCollection`](../../outlinecodecollection/) 객체를 가져오거나 설정합니다.

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## 비고

두 개의 데이터가 필요합니다 - FieldID로 지정된 개요 코드 테이블에 대한 포인터와 ValueID 또는 ValueGUID로 지정된 값 리스트에 대한 포인터 중 하나.

## 예제

작업의 개요 코드 값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### 또 보기

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


