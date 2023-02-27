---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Aspose.Tasks för .NET API-referens
description: ProjectServerCredentials byggare. Initierar en ny instans avProjectServerCredentials klass med URL till SharePointwebbplats och giltig SPOIDCRLauktoriseringstoken för SharePoints PWAwebbplats Project Web Access.
type: docs
weight: 10
url: /sv/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Initierar en ny instans av[`ProjectServerCredentials`](../) klass med URL till SharePoint-webbplats och giltig SPOIDCRL-auktoriseringstoken för SharePoints PWA-webbplats (Project Web Access).

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| siteUrl | String | URL:en för PWA (Project Web Access) API för Project Online. |
| authToken | String | Auktoriseringstoken (SPOIDCRL) för SharePoints PWA-webbplats (Project Web Access). |

### Anmärkningar

Använd denna konstruktor för att ansluta till ProjectOnline när du redan har AuthToken för din SharePoint Online-webbplats.

### Se även

* class [ProjectServerCredentials](../)
* namnutrymme [Aspose.Tasks](../../projectservercredentials/)
* hopsättning [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Initierar en ny instans av[`ProjectServerCredentials`](../) klass med URL till SharePoint-webbplats, användarnamn och lösenord.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| siteUrl | String | URL:en för PWA (Project Web Access) API för Project Online. |
| userName | String | Användarnamnet för SharePoint-webbplatsen. |
| password | String | Lösenordet för SharePoint-webbplatsen. |

### Anmärkningar

Använd den här konstruktören för att ansluta till ProjectOnline. Observera att äldre autentisering bör vara aktiverad i din Azure-portal och Office 365 Admin Center.

### Se även

* class [ProjectServerCredentials](../)
* namnutrymme [Aspose.Tasks](../../projectservercredentials/)
* hopsättning [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Initierar en ny instans av[`ProjectServerCredentials`](../) klass med hjälp av URL till Project Web Access-slutpunkt och nätverksuppgifter.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| siteUrl | String | Webbadressen för projektets webbåtkomstslutpunkt. |
| credentials | NetworkCredential | Autentiseringsuppgifterna som används för att logga in på Project Web Access-slutpunkten. |

### Anmärkningar

Använd den här konstruktorn för att ansluta till den lokala instansen av Project Server via PWA.

### Exempel

I det här exemplet instansen av[`ProjectServerManager`](../../projectservermanager/)klass används för att läsa en lista över projekt från Project Server-instansen som finns på http://project_server_instance.local

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

### Se även

* class [ProjectServerCredentials](../)
* namnutrymme [Aspose.Tasks](../../projectservercredentials/)
* hopsättning [Aspose.Tasks](../../../)


