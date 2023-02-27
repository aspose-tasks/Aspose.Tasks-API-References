---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Aspose.Tasks for .NET API Referansı
description: ProjectServerCredentials inşaatçı. Yeni bir örneğini başlatır.ProjectServerCredentials SharePoint sitesinin URLsini ve SharePointin PWA Proje Web Erişimi sitesi için geçerli SPIDCRL yetkilendirme belirtecini kullanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Yeni bir örneğini başlatır.[`ProjectServerCredentials`](../) SharePoint sitesinin URL'sini ve SharePoint'in PWA (Proje Web Erişimi) sitesi için geçerli SPIDCRL yetkilendirme belirtecini kullanan sınıf.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| siteUrl | String | Project Online'ın PWA (Project Web Erişimi) API'sinin URL'si. |
| authToken | String | SharePoint'in PWA (Proje Web Erişimi) sitesi için yetkilendirme belirteci (SPIDCRL). |

### Notlar

SharePoint Online siteniz için zaten AuthToken'a sahip olduğunuzda ProjectOnline'a bağlanmak için bu oluşturucuyu kullanın.

### Ayrıca bakınız

* class [ProjectServerCredentials](../)
* ad alanı [Aspose.Tasks](../../projectservercredentials/)
* toplantı [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Yeni bir örneğini başlatır.[`ProjectServerCredentials`](../) SharePoint sitesinin URL'sini, kullanıcı adını ve parolayı kullanan sınıf.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| siteUrl | String | Project Online'ın PWA (Project Web Erişimi) API'sinin URL'si. |
| userName | String | SharePoint sitesinin kullanıcı adı. |
| password | String | SharePoint sitesinin parolası. |

### Notlar

ProjectOnline'a bağlanmak için bu oluşturucuyu kullanın. Azure portalınızda ve Office 365 Yönetici merkezinizde eski kimlik doğrulamanın etkinleştirilmesi gerektiğini lütfen unutmayın.

### Ayrıca bakınız

* class [ProjectServerCredentials](../)
* ad alanı [Aspose.Tasks](../../projectservercredentials/)
* toplantı [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Yeni bir örneğini başlatır.[`ProjectServerCredentials`](../) Project Web Access uç noktası URL'sini ve ağ kimlik bilgilerini kullanan sınıf.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| siteUrl | String | Proje web erişimi uç noktasının URL'si. |
| credentials | NetworkCredential | Project Web Access uç noktasında oturum açmak için kullanılan kimlik bilgileri. |

### Notlar

PWA aracılığıyla şirket içi Project Server örneğine bağlanmak için bu oluşturucuyu kullanın.

### Örnekler

Bu örnekte örneği[`ProjectServerManager`](../../projectservermanager/)sınıf, http://project_server_instance.local adresinde bulunan Project Server örneğinden bir proje listesi okumak için kullanılır.

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

### Ayrıca bakınız

* class [ProjectServerCredentials](../)
* ad alanı [Aspose.Tasks](../../projectservercredentials/)
* toplantı [Aspose.Tasks](../../../)


