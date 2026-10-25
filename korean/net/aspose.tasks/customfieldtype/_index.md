---
title: "Enum CustomFieldType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CustomFieldType enum. 사용자 정의 필드의 유형을 지정합니다."
type: docs
weight: 380
url: /ko/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

사용자 정의 필드 유형을 지정합니다.

```csharp
public enum CustomFieldType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Null | `0` | Null 사용자 정의 필드 유형을 나타냅니다. |
| Cost | `1` | Cost 사용자 정의 필드 유형을 나타냅니다. |
| Date | `2` | Date 사용자 정의 필드 유형을 나타냅니다. |
| Duration | `3` | Duration 사용자 정의 필드 유형을 나타냅니다. |
| Finish | `4` | Finish 사용자 정의 필드 유형을 나타냅니다. |
| Flag | `5` | Flag 사용자 정의 필드 유형을 나타냅니다. |
| Number | `6` | Number 사용자 정의 필드 유형을 나타냅니다. |
| Start | `7` | Start 사용자 정의 필드 유형을 나타냅니다. |
| Text | `8` | Text 사용자 정의 필드 유형을 나타냅니다. |
| OutlineCode | `9` | Outline Code 사용자 정의 필드 유형을 나타냅니다. |
| RBS | `10` | RBS (Resource Breakdown Structure) 사용자 정의 필드 유형을 나타냅니다. |

## 예제

사용 방법을 보여줍니다 &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// 정의와 작업합니다...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


