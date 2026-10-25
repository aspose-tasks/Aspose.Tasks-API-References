---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ProjectServerCredentials. يهيئ مثيلًا جديدًا من فئة ProjectServerCredentials باستخدام عنوان URL لموقع SharePoint ورمز تفويض SPOIDCRL صالح لموقع PWA الخاص بـ SharePoint"
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

يُهيئ مثيلًا جديدًا من الفئة [`ProjectServerCredentials`](../) باستخدام عنوان URL لموقع SharePoint ورمز تفويض SPOIDCRL صالح لموقع PWA (Project Web Access) الخاص بـ SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| siteUrl | سلسلة | عنوان URL لواجهة برمجة تطبيقات PWA (Project Web Access) في Project Online. |
| authToken | سلسلة | رمز التفويض (SPOIDCRL) لموقع PWA (Project Web Access) الخاص بـ SharePoint. |

## ملاحظات

استخدم هذا المُنشئ للاتصال بـ ProjectOnline عندما يكون لديك بالفعل AuthToken لموقع SharePoint Online الخاص بك.

## الأمثلة

يوضح كيفية استخدام بيانات اعتماد Project Server مع SharePointOnlineCredentials لإنشاء مشروع في Microsoft Project Online.

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

### انظر أيضًا

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

ينشئ مثلاً جديداً من الفئة [`ProjectServerCredentials`](../) باستخدام عنوان URL لموقع SharePoint، اسم المستخدم وكلمة المرور.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| siteUrl | سلسلة | عنوان URL لواجهة برمجة تطبيقات PWA (Project Web Access) في Project Online. |
| userName | سلسلة | اسم المستخدم لموقع SharePoint. |
| password | سلسلة | كلمة المرور لموقع SharePoint. |

## ملاحظات

استخدم هذا المُنشئ للاتصال بـ ProjectOnline. يرجى ملاحظة أنه يجب تمكين المصادقة القديمة في بوابة Azure ومركز إدارة Office 365.

## الأمثلة

يعرض كيفية استخدام بيانات اعتماد خادم المشروع لاسترجاع قائمة المشاريع من Microsoft Project Online.

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

### انظر أيضًا

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

ينشئ مثلاً جديداً من الفئة [`ProjectServerCredentials`](../) باستخدام عنوان URL لنقطة نهاية Project Web Access وبيانات الاعتماد الشبكية.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| siteUrl | سلسلة | عنوان URL لنقطة نهاية Project Web Access. |
| بيانات الاعتماد | NetworkCredential | بيانات الاعتماد المستخدمة لتسجيل الدخول إلى نقطة نهاية Project Web Access. |

## ملاحظات

استخدم هذا المُنشئ للاتصال بنسخة Project Server المحلية عبر PWA.

## الأمثلة

في هذا المثال يتم استخدام مثيل الفئة [`ProjectServerManager`](../../projectservermanager/) لقراءة قائمة بالمشروعات من نسخة Project Server الموجودة على http://project_server_instance.local

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

يوضح كيفية استخدام بيانات اعتماد Project Server مع بيانات الاعتماد الشبكية لقراءة مشروع من نسخة Project Server المحلية.

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

### انظر أيضًا

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


