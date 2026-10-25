---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks for .NET API 참조"
description: "LoadOptions 속성. 프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 가져오거나 설정합니다.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## 예제

CancellationToken을 전달하여 장시간 실행되는 프로젝트 로드 작업을 취소하는 방법을 보여줍니다.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts는 다른 스레드에 전달될 수 있으며, 해당 스레드에서 cts.Cancel() 메서드를 호출하여 프로젝트 로드 작업을 취소할 수 있습니다.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### 또 보기

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


