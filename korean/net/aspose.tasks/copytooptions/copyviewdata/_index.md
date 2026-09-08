---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CopyToOptions 속성. 프로젝트 데이터를 복사하는 동안 뷰 데이터를 복사할지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 true입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

프로젝트 데이터를 복사하는 동안 보기 데이터를 복사할지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은 true입니다.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


