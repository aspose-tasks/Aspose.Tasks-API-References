---
title: "Aspose::Tasks::Metered class"
linktitle: "계량된"
articleTitle: "계량된"
second_title: "C++용 Aspose.Tasks"
description: "계량 키를 설정하는 메서드를 제공합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/metered/
---

## Metered class

계량 키를 설정하는 메서드를 제공합니다.

이 예제에서는 계량된 공개 및 개인 키 <ms>를 설정하려고 시도합니다.

```cpp
[C#]
 
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
 
 
[Visual Basic]
 
Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

</ms> <java> 구성 요소 jar 파일:

```cpp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

</java>

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetConsumptionCredit](./getconsumptioncredit/) | 소비 크레딧을 가져옵니다. |
| [GetConsumptionQuantity](./getconsumptionquantity/) | 소비 파일 크기를 가져옵니다. |
| [IsLicensed](./islicensed/) | Metered 라이선스를 사용하여 제품이 성공적으로 라이선스가 부여되었는지 확인합니다. |
| [ResetMeteredKey](./resetmeteredkey/) | 이전에 설정된 라이선스를 제거합니다. |
| [SetMeteredKey](./setmeteredkey/) | Metered 공개 및 개인 키를 설정합니다. |

