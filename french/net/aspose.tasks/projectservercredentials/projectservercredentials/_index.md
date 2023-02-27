---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ProjectServerCredentials constructeur. Initialise une nouvelle instance duProjectServerCredentials classe utilisant lURL du site SharePoint et un jeton dautorisation SPOIDCRL valide pour le site PWA Project Web Access de SharePoint.
type: docs
weight: 10
url: /fr/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Initialise une nouvelle instance du[`ProjectServerCredentials`](../) classe utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| siteUrl | String | L'URL de l'API PWA (Project Web Access) de Project Online. |
| authToken | String | Le jeton d'autorisation (SPOIDCRL) pour le site PWA (Project Web Access) de SharePoint. |

### Remarques

Utilisez ce constructeur pour vous connecter à ProjectOnline lorsque vous disposez déjà d'AuthToken pour votre site SharePoint Online.

### Voir également

* class [ProjectServerCredentials](../)
* espace de noms [Aspose.Tasks](../../projectservercredentials/)
* Assemblée [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Initialise une nouvelle instance du[`ProjectServerCredentials`](../) classe en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| siteUrl | String | L'URL de l'API PWA (Project Web Access) de Project Online. |
| userName | String | Le nom d'utilisateur pour le site SharePoint. |
| password | String | Le mot de passe du site SharePoint. |

### Remarques

Utilisez ce constructeur pour vous connecter à ProjectOnline. Veuillez noter que l'authentification héritée doit être activée dans votre portail Azure et votre centre d'administration Office 365.

### Voir également

* class [ProjectServerCredentials](../)
* espace de noms [Aspose.Tasks](../../projectservercredentials/)
* Assemblée [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Initialise une nouvelle instance du[`ProjectServerCredentials`](../) classe à l'aide de l'URL du point de terminaison Project Web Access et des informations d'identification réseau.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| siteUrl | String | URL du point de terminaison d'accès Web du projet. |
| credentials | NetworkCredential | Les informations d'identification utilisées pour se connecter au point de terminaison Project Web Access. |

### Remarques

Utilisez ce constructeur pour vous connecter à une instance locale de Project Server via PWA.

### Exemples

Dans cet exemple, l'instance de[`ProjectServerManager`](../../projectservermanager/)la classe est utilisée pour lire une liste de projets à partir de l'instance de Project Server située à http://project_server_instance.local

```csharp
string site = "http://project_server_instance.local/sites/pwa" ;
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

### Voir également

* class [ProjectServerCredentials](../)
* espace de noms [Aspose.Tasks](../../projectservercredentials/)
* Assemblée [Aspose.Tasks](../../../)


