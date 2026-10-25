---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "CopyToOptions 생성자. CopyToOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

[`CopyToOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public CopyToOptions()
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


