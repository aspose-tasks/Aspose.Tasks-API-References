---
title: "열거형 WorkGroupType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkGroupType 열거형. 작업 그룹의 유형을 지정합니다"
type: docs
weight: 3620
url: /ko/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

작업 그룹의 유형을 지정합니다.

```csharp
public enum WorkGroupType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Default | `0` | 기본 작업 그룹 유형을 나타냅니다. |
| None | `1` | 없음 작업 그룹 유형을 나타냅니다. |
| Email | `2` | 이메일 작업 그룹 유형을 나타냅니다. |
| Web | `3` | 웹 작업 그룹 유형을 나타냅니다. |

## 예제

리소스의 작업 그룹을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


