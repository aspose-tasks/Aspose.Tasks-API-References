---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. OutlineCodeCollection 개체를 가져옵니다. 개요 코드의 값"
type: docs
weight: 540
url: /ko/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

OutlineCodeCollection 객체를 가져옵니다. 개요 코드의 값입니다.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## 비고

두 개의 데이터가 필요합니다 - FieldID로 지정된 개요 코드 테이블에 대한 포인터와 ValueID 또는 ValueGUID로 지정된 값 리스트에 대한 포인터 중 하나.

## 예제

리소스 개요 값을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### 또 보기

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


