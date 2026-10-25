---
title: "클래스 LoadOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.LoadOptions 클래스. 파일이나 스트림에서 프로젝트를 로드할 때 추가 로드 매개변수를 지정할 수 있습니다."
type: docs
weight: 990
url: /ko/net/aspose.tasks/loadoptions/
---
## LoadOptions class

파일이나 스트림에서 프로젝트를 로드할 때 추가 로드 매개변수를 지정할 수 있습니다.

```csharp
public class LoadOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [LoadOptions](loadoptions/)() | `LoadOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | 프로젝트 로드 작업을 취소하는 데 사용할 수 있는 토큰을 가져오거나 설정합니다. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | HTML, MPX, XER 및 Primavera XML 형식에서 프로젝트를 읽는 데 사용되는 인코딩을 가져오거나 설정합니다. 기본 인코딩은 UTF8입니다. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | XML 구문 분석 오류를 처리하기 위한 콜백 메서드를 가져오거나 설정합니다. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | 보호 비밀번호를 가져오거나 설정합니다. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | [`PrimaveraReadOptions`](../primaverareadoptions/) 클래스의 지정된 인스턴스를 가져오거나 설정합니다. 이 인스턴스는 Primavera 형식(Primavera P6 XER 또는 Primavera P6 Xml) 로드 동작을 사용자 지정하는 데 사용할 수 있습니다. |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | 프로젝트 로드 작업 중에 호출되는 콜백을 가져오거나 설정합니다. 현재 MPP 및 XER 형식을 지원합니다. |

## 예제

<see cref="Aspose.Tasks.LoadOptions"/> 인스턴스를 사용하여 비밀번호로 보호된 프로젝트를 로드하는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


