---
title: "License.License"
second_title: "Aspose.Tasks for .NET API 참조"
description: "License 생성자. License 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/license/license/
---
## License constructor

[`License`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public License()
```

## 예제

이 예제에서는 구성 요소가 포함된 폴더, 호출 어셈블리가 포함된 폴더, 진입 어셈블리 폴더, 그리고 호출 어셈블리의 임베디드 리소스에서 MyLicense.lic이라는 라이선스 파일을 찾으려고 시도합니다.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

구성 요소 jar 파일:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Aspose.Tasks의 라이선스를 적용하는 방법을 보여줍니다.

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### 또 보기

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


