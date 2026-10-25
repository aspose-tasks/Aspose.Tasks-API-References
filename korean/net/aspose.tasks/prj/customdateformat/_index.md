---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 프로젝트 보기 사용자 지정 날짜 형식. DateFormat 속성이 Custom으로 설정된 경우 날짜를 형식화하는 데 사용됩니다."
type: docs
weight: 200
url: /ko/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

프로젝트 보기 사용자 지정 날짜 형식. [`DateFormat`](../dateformat/) 속성이 Custom으로 설정된 경우 날짜를 형식화하는 데 사용됩니다.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## 예제

Prj.CustomDateFormat 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


