---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerCredentials कंस्ट्रक्टर। SharePoint साइट का URL और वैध SPOIDCRL ऑथराइज़ेशन टोकन का उपयोग करके ProjectServerCredentials क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है, जो SharePoints PWA Project Web Access साइट के लिए है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

SharePoint साइट का URL और वैध SPOIDCRL ऑथराइज़ेशन टोकन का उपयोग करके [`ProjectServerCredentials`](../) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है, जो SharePoint के PWA (Project Web Access) साइट के लिए है।

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| siteUrl | स्ट्रिंग | Project Online के PWA (Project Web Access) API का URL। |
| authToken | स्ट्रिंग | SharePoint की PWA (Project Web Access) साइट के लिए प्राधिकरण टोकन (SPOIDCRL) । |

## टिप्पणियाँ

जब आपके पास SharePoint Online साइट के लिए AuthToken हो, तब ProjectOnline से कनेक्ट करने के लिए इस कंस्ट्रक्टर का उपयोग करें।

## उदाहरण

दिखाता है कि कैसे Project Server क्रेडेंशियल्स को SharePointOnlineCredentials के साथ उपयोग करके Microsoft Project Online में प्रोजेक्ट बनाया जाए।

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

### संबंधित देखें

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

`[`ProjectServerCredentials`](../)` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, जिसमें SharePoint साइट का URL, उपयोगकर्ता नाम और पासवर्ड उपयोग किए जाते हैं।

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| siteUrl | स्ट्रिंग | Project Online के PWA (Project Web Access) API का URL। |
| userName | स्ट्रिंग | SharePoint साइट के लिए उपयोगकर्ता नाम। |
| password | स्ट्रिंग | SharePoint साइट के लिए पासवर्ड। |

## टिप्पणियाँ

ProjectOnline से कनेक्ट करने के लिए इस कंस्ट्रक्टर का उपयोग करें। कृपया ध्यान दें कि लेगेसी ऑथेंटिकेशन को आपके Azure पोर्टल और Office 365 एडमिन सेंटर में सक्षम होना चाहिए।

## उदाहरण

विवरण देता है कि Microsoft Project Online से प्रोजेक्ट की सूची प्राप्त करने के लिए प्रोजेक्ट सर्वर क्रेडेंशियल्स का उपयोग कैसे करें।

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

### संबंधित देखें

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

`[`ProjectServerCredentials`](../)` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, जिसमें Project Web Access एंडपॉइंट का URL और नेटवर्क क्रेडेंशियल्स उपयोग किए जाते हैं।

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| siteUrl | स्ट्रिंग | Project Web Access एंडपॉइंट का URL। |
| क्रेडेंशियल्स | NetworkCredential | Project Web Access एंडपॉइंट में लॉगिन करने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स। |

## टिप्पणियाँ

PWA के माध्यम से Project Server के ऑन-प्रिमाइसेस इंस्टेंस से कनेक्ट करने के लिए इस कंस्ट्रक्टर का उपयोग करें।

## उदाहरण

इस उदाहरण में, [`ProjectServerManager`](../../projectservermanager/) क्लास का इंस्टेंस उपयोग किया गया है, जो http://project_server_instance.local पर स्थित Project Server इंस्टेंस से प्रोजेक्ट की सूची पढ़ता है।

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

दिखाता है कि ऑन-प्रिमाइसेस Project Server इंस्टेंस से प्रोजेक्ट पढ़ने के लिए Project Server क्रेडेंशियल्स को नेटवर्क क्रेडेंशियल्स के साथ कैसे उपयोग किया जाए।

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

### संबंधित देखें

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


