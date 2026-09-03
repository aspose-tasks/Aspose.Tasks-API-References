---
title: "Aspose::Tasks::License 클래스"
linktitle: "라이선스"
articleTitle: "라이선스"
second_title: "C++용 Aspose.Tasks"
description: "구성 요소에 라이선스를 부여하는 메서드를 제공합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/license/
---

## License class

구성 요소에 라이선스를 부여하는 메서드를 제공합니다.

이 예제에서는 <ms> 구성 요소가 포함된 폴더, 호출 어셈블리가 포함된 폴더, 진입 어셈블리 폴더에서 MyLicense.lic 라는 라이선스 파일을 찾으려고 시도합니다. 그리고 마지막으로 호출 어셈블리의 임베디드 리소스에서 찾습니다.

```cpp
[C#]
 
License license = new License();
license.SetLicense("MyLicense.lic");
 
 
[Visual Basic]
 
Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

</ms> <java> 구성 요소 jar 파일:

```cpp
License license = new License();
license.setLicense("MyLicense.lic");
```

</java>

## 생성자

| 이름 | 설명 |
| --- | --- |
| [License](./license/) | License 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [SetLicense (2 overloads)](./setlicense/) | 구성 요소에 라이선스를 적용합니다. |

