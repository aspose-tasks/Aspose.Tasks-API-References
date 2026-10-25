---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 메서드. 기본 저장 옵션을 사용하여 Project ServerProject Online 인스턴스에 새 프로젝트를 생성합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

기본 저장 옵션을 사용하여 Project Server\Project Online 인스턴스에 새 프로젝트를 생성합니다.

```csharp
public void CreateNewProject(Project project)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트. |

### 예외

| 예외 | 조건 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류가 발생하거나 서버에서 오류가 반환된 경우. |

## 예제

이 예제에서는 프로젝트를 .mpp 파일에서 로드하고 Project Online 계정에 저장합니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Microsoft Project Online에서 새 프로젝트를 생성하기 위해 ProjectServerManager를 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 프로젝트 | Project | Project Server\Project Online 인스턴스에 저장할 프로젝트. |
| saveOptions | ProjectServerSaveOptions | [`ProjectServerSaveOptions`](../../projectserversaveoptions/) 클래스의 인스턴스. |

### 예외

| 예외 | 조건 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 통신 오류가 발생하거나 서버에서 오류가 반환된 경우. |

## 예제

이 예제에서는 프로젝트를 .mpp 파일에서 로드하고 Project Online 계정에 저장합니다.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

Microsoft Project Online에서 미리 정의된 저장 옵션으로 새 프로젝트를 만들기 위해 Project Server 관리자를 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


