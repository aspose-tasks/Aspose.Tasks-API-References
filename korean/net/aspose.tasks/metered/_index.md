---
title: "클래스 Metered"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Metered 클래스. 메터링 키를 설정하는 메서드를 제공합니다"
type: docs
weight: 1020
url: /ko/net/aspose.tasks/metered/
---
## Metered class

계량 키를 설정하는 메서드를 제공합니다.

```csharp
public class Metered
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Metered](metered/)() | 기본 생성자입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | 메터링 라이선스를 사용하여 제품이 성공적으로 라이선스가 부여되었는지 확인합니다. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | 이전에 설정된 라이선스를 제거합니다. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | 메터링 공개 및 개인 키를 설정합니다. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | 소비 크레딧을 가져옵니다. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | 소비 파일 크기를 가져옵니다. |

## 예제

이 예제에서는 메터링 공개 및 개인 키를 설정하려고 시도합니다.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

구성 요소 jar 파일:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


