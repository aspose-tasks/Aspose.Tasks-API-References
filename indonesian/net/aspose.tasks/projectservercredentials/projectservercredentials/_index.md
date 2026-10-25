---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ProjectServerCredentials konstruktor. Menginisialisasi instance baru dari kelas ProjectServerCredentials menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk situs PWA Project Web Access SharePoint"
type: docs
weight: 10
url: /id/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Menginisialisasi instance baru dari kelas [`ProjectServerCredentials`](../) menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk PWA (Project Web Access) situs SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| siteUrl | String | URL PWA (Project Web Access) API dari Project Online. |
| authToken | String | Token otorisasi (SPOIDCRL) untuk situs PWA (Project Web Access) SharePoint. |

## Catatan

Gunakan konstruktor ini untuk terhubung ke ProjectOnline ketika Anda sudah memiliki AuthToken untuk situs SharePoint Online Anda.

## Contoh

Menampilkan cara menggunakan kredensial Project Server dengan SharePointOnlineCredentials untuk membuat proyek di Microsoft Project Online.

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

### Lihat Juga

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Menginisialisasi instance baru dari kelas [`ProjectServerCredentials`](../) menggunakan URL situs SharePoint, nama pengguna, dan kata sandi.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| siteUrl | String | URL PWA (Project Web Access) API dari Project Online. |
| userName | String | Nama pengguna untuk situs SharePoint. |
| password | String | Kata sandi untuk situs SharePoint. |

## Catatan

Gunakan konstruktor ini untuk terhubung ke ProjectOnline. Harap perhatikan bahwa otentikasi lama harus diaktifkan di portal Azure Anda dan pusat admin Office 365.

## Contoh

Menampilkan cara menggunakan kredensial project server untuk mengambil daftar proyek dari Microsoft Project Online.

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

### Lihat Juga

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Menginisialisasi instance baru dari kelas [`ProjectServerCredentials`](../) menggunakan URL endpoint Project Web Access dan kredensial jaringan.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| siteUrl | String | URL endpoint project web access. |
| kredensial | NetworkCredential | Kredensial yang digunakan untuk masuk ke endpoint Project Web Access. |

## Catatan

Gunakan konstruktor ini untuk terhubung ke instance on-premise Project Server melalui PWA.

## Contoh

Dalam contoh ini, instance dari kelas [`ProjectServerManager`](../../projectservermanager/) digunakan untuk membaca daftar proyek dari instance Project Server yang terletak di http://project_server_instance.local

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

Menampilkan cara menggunakan kredensial Project Server dengan kredensial jaringan untuk membaca proyek dari instance on-premise Project Server.

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

### Lihat Juga

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


