---
title: "클래스 CopyToOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CopyToOptions 클래스. 프로젝트 데이터를 복사할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 340
url: /ko/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

프로젝트 데이터를 복사할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class CopyToOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CopyToOptions](copytooptions/)() | `CopyToOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | 프로젝트 데이터를 복사하는 동안 보기 데이터를 복사할지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 true입니다. |

## 예제

프로젝트 복사 옵션 사용 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// 공통 프로젝트 데이터를 복사하는 동안 보기 데이터 복사를 건너뜁니다.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


