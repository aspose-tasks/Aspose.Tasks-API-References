---
title: "Project.Get"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 이 컨테이너에서 속성이 매핑된 값을 반환합니다"
type: docs
weight: 1080
url: /ko/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

이 컨테이너에서 속성이 매핑된 값을 반환합니다.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 매핑된 값의 유형. |
| key | 지정된 속성 키. [`Prj`](../../prj/)는 속성 키를 가져오기 위해 사용됩니다. |

### 반환 값

속성이 이 컨테이너에 매핑되는 값.

## 예제

프로젝트 버전을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// 프로젝트 버전 표시
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


