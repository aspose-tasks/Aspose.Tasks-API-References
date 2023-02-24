---
title: Class ProjectServerCredentials
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.ProjectServerCredentials classe. Identifiants utilisés pour se connecter à Project Online ou à une instance locale de Project Server.
type: docs
weight: 1240
url: /fr/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Identifiants utilisés pour se connecter à Project Online ou à une instance locale de Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Initialise une nouvelle instance du`ProjectServerCredentials` classe à l'aide de l'URL du point de terminaison Project Web Access et des informations d'identification réseau. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Initialise une nouvelle instance du`ProjectServerCredentials` classe utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Initialise une nouvelle instance du`ProjectServerCredentials` classe en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Obtient le jeton d'autorisation pour l'instance SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Obtient l'URL de PWA sur le site SharePoint ou l'URL de Project Server sur site. Par exemple, https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Obtient le nom d'utilisateur pour le site SharePoint. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Renvoie une représentation sous forme de chaîne de cette instance. |

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


