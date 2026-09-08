---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerCredentials 생성자. SharePoint 사이트의 URL과 SharePoint의 PWA Project Web Access 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 ProjectServerCredentials 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

[`ProjectServerCredentials`](../) 클래스의 새 인스턴스를 SharePoint 사이트의 URL과 SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 유효한 SPOIDCRL 인증 토큰을 사용하여 초기화합니다.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| siteUrl | 문자열 | Project Online의 PWA(프로젝트 웹 액세스) API URL입니다. |
| authToken | 문자열 | SharePoint의 PWA(프로젝트 웹 액세스) 사이트에 대한 인증 토큰(SPOIDCRL)입니다. |

## 비고

이미 SharePoint Online 사이트에 대한 AuthToken이 있는 경우 이 생성자를 사용하여 ProjectOnline에 연결합니다.

## 예제

Project Server 자격 증명을 SharePointOnlineCredentials와 함께 사용하여 Microsoft Project Online에서 프로젝트를 만드는 방법을 보여줍니다.

```csharp
try
{
    const string Username = "admin@contoso.onmicrosoft.com";
    const string SecuredPassword = "MyPassword";
    var url = new Uri("https://contoso.sharepoint.com/sites/pwa");
    var project = new Project(DataDir + "Project1.mpp");
    var password = new SecureString();
    foreach (var c in SecuredPassword)
    {
        password.AppendChar(c);
    }

    var onlineCredentials = new SharePointOnlineCredentials(Username, password);
    var projectServerCredentials = new ProjectServerCredentials(url.ToString(), onlineCredentials.GetAuthenticationCookie(url, true));

    Console.WriteLine("Project Server Auth Token: " + projectServerCredentials.AuthToken);
    Console.WriteLine("Project Server Site Url: " + projectServerCredentials.SiteUrl);
    Console.WriteLine("Project Server User Name: " + projectServerCredentials.UserName);

    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

SharePoint 사이트의 URL, 사용자 이름 및 비밀번호를 사용하여 [`ProjectServerCredentials`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| siteUrl | 문자열 | Project Online의 PWA(프로젝트 웹 액세스) API URL입니다. |
| userName | 문자열 | SharePoint 사이트의 사용자 이름입니다. |
| password | 문자열 | SharePoint 사이트의 비밀번호입니다. |

## 비고

이 생성자를 사용하여 ProjectOnline에 연결합니다. 레거시 인증은 Azure 포털 및 Office 365 관리 센터에서 활성화되어야 함을 참고하십시오.

## 예제

Microsoft Project Online에서 프로젝트 목록을 검색하기 위해 프로젝트 서버 자격 증명을 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Project Web Access 엔드포인트의 URL과 네트워크 자격 증명을 사용하여 [`ProjectServerCredentials`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| siteUrl | 문자열 | Project Web Access 엔드포인트의 URL입니다. |
| 자격 증명 | NetworkCredential | Project Web Access 엔드포인트에 로그인하는 데 사용되는 자격 증명입니다. |

## 비고

PWA를 통해 온프레미스 Project Server 인스턴스에 연결하려면 이 생성자를 사용합니다.

## 예제

이 예제에서는 [`ProjectServerManager`](../../projectservermanager/) 클래스의 인스턴스를 사용하여 http://project_server_instance.local에 위치한 Project Server 인스턴스에서 프로젝트 목록을 읽습니다.

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

온프레미스 Project Server 인스턴스에서 프로젝트를 읽기 위해 네트워크 자격 증명과 함께 Project Server 자격 증명을 사용하는 방법을 보여줍니다.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


