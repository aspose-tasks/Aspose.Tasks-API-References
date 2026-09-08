---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Metered 메서드. Metered 공개 및 개인 키를 설정합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

메터링 공개 및 개인 키를 설정합니다.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| publicKey | 문자열 | 공개 키. |
| privateKey | 문자열 | 개인 키. |

## 비고

계량형 라이선스를 구매한 경우, 이 API는 애플리케이션 시작 시 호출되어야 하며 일반적으로 이것만으로 충분합니다. 그러나 계량형이 24시간 동안 사용량 데이터를 업로드하지 못하면 라이선스가 평가 상태로 설정됩니다. 이러한 경우를 방지하려면 라이선스 상태를 정기적으로 확인해야 하며, 평가 상태인 경우 이 API를 다시 호출하십시오.

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


