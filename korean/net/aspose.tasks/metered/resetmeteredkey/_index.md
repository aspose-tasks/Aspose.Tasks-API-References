---
title: "Metered.ResetMeteredKey"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Metered 메서드. 이전에 설정된 라이선스를 제거합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/metered/resetmeteredkey/
---
## Metered.ResetMeteredKey method

이전에 설정된 라이선스를 제거합니다.

```csharp
public void ResetMeteredKey()
```

## 예제

Aspose.Tasks와 함께 &lt;see cref=\"Aspose.Tasks.Metered\" /&gt; 라이선스 유형을 사용하는 방법을 보여줍니다.

```csharp
// metered 라이선스를 사용해 봅시다 (see https://purchase.aspose.com/faqs/licensing/metered)
// metered 라이선스 설정
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// 프로젝트 작업...
// ...

// 현재 크레딧 및 바이트 사용량을 가져올 수 있습니다.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // 예외 로그
}

// 최근 사용자는 metered를 재설정하고 바이트 카운트를 중지할 수 있습니다.
metered.ResetMeteredKey();
```

### 또 보기

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


