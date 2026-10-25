---
title: "License.SetLicense"
second_title: "Aspose.Tasks for .NET API 참조"
description: "License 메서드. 구성 요소에 라이선스를 적용합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

구성 요소에 라이선스를 적용합니다.

```csharp
public void SetLicense(string licenseName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| licenseName | 문자열 | 전체 파일 이름이거나 짧은 파일 이름, 또는 포함된 리소스의 이름일 수 있습니다. 빈 문자열을 사용하면 평가 모드로 전환됩니다. |

## 비고

다음 위치에서 라이선스를 찾으려고 시도합니다:

1. 명시적 경로.

2. Aspose 구성 요소 어셈블리가 포함된 폴더.

3. 클라이언트의 호출 어셈블리가 포함된 폴더.

4. 엔트리(시작) 어셈블리가 포함된 폴더.

5. 클라이언트의 호출 어셈블리에 포함된 리소스.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 명시적 경로.

2. 클라이언트의 호출 어셈블리에 포함된 리소스.

2. Aspose 구성 요소 JAR 파일이 포함된 폴더.

3. 클라이언트의 호출 JAR 파일이 포함된 폴더.

## 예제

이 예제에서는 구성 요소가 포함된 폴더, 호출 어셈블리가 포함된 폴더, 진입 어셈블리 폴더, 그리고 호출 어셈블리의 임베디드 리소스에서 MyLicense.lic이라는 라이선스 파일을 찾으려고 시도합니다.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

---

## SetLicense(Stream) {#setlicense}

구성 요소에 라이선스를 적용합니다.

```csharp
public void SetLicense(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 라이선스를 포함하는 스트림. |

## 비고

이 메서드를 사용하여 스트림에서 라이선스를 로드합니다.

## 예제

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

Aspose.Tasks의 라이선스를 &lt;see cref=\"System.IO.FileStream\" /&gt;에서 읽어 적용하는 방법을 보여줍니다.

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### 또 보기

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


