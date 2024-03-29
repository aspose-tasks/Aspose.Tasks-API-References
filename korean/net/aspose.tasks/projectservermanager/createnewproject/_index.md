---
title: CreateNewProject
second_title: .NET API 참조용 Aspose.Tasks
description: 기본 저장 옵션을 사용하여 Project ServerProject Online 인스턴스에 새 프로젝트를 만듭니다.
type: docs
weight: 30
url: /ko/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

기본 저장 옵션을 사용하여 Project Server\Project Online 인스턴스에 새 프로젝트를 만듭니다.

```csharp
public void CreateNewProject(Project project)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| project | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류 또는 서버에서 반환된 오류의 경우. |

### 예

이 예에서 프로젝트는 .mpp 파일에서 로드되고 Project Online 계정에 저장됩니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "암호");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

### 또한보십시오

* class [Project](../../project/)
* class [ProjectServerManager](../)
* 네임스페이스 [Aspose.Tasks](../../projectservermanager/)
* 집회 [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

지정된 저장 옵션을 사용하여 Project Server\Project Online 인스턴스에 새 프로젝트를 만듭니다.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| project | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트입니다. |
| saveOptions | ProjectServerSaveOptions | 대신에[`ProjectServerSaveOptions`](../../projectserversaveoptions/) 수업. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류 또는 서버에서 반환된 오류의 경우. |

### 예

이 예에서 프로젝트는 .mpp 파일에서 로드되고 Project Online 계정에 저장됩니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "암호");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

### 또한보십시오

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* 네임스페이스 [Aspose.Tasks](../../projectservermanager/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
