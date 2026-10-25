---
title: "Project.CopyTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다."
type: docs
weight: 1060
url: /ko/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다.

```csharp
public void CopyTo(Project another)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | Project | 데이터를 복사할 다른 프로젝트입니다. |

## 예제

프로젝트 데이터를 다른 프로젝트로 복사하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// 공통 프로젝트 데이터를 복사하는 동안 보기 데이터 복사를 건너뜁니다.
project.CopyTo(mppProject);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

프로젝트의 주요 데이터와 속성을 다른 프로젝트에 복사합니다.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | Project | 데이터를 복사할 다른 프로젝트입니다. |
| 옵션 | CopyToOptions | 복사 프로세스를 제어하기 위한 복사 옵션. |

## 예제

&lt;see cref=\"Aspose.Tasks.CopyToOptions\"/&gt; 인스턴스를 사용하여 프로젝트를 복사하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// 공통 프로젝트 데이터를 복사하는 동안 보기 데이터 복사를 건너뜁니다.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### 또 보기

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


