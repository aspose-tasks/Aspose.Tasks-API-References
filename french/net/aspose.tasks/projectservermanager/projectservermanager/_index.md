---
title: ProjectServerManager.ProjectServerManager
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ProjectServerManager constructeur. Initialise une nouvelle instance duProjectServerManager classe.
type: docs
weight: 10
url: /fr/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Initialise une nouvelle instance du[`ProjectServerManager`](../) classe.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Identifiants utilisés pour se connecter au compte Project Online. |

### Exemples

Cet exemple montre comment créer une instance de ProjectServerManager pour accéder à une instance sur site de Project Server.

```csharp
[C#]
string site = "http://instance_serveur_projet.local/" ;
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Cet exemple montre comment créer une instance de ProjectServerManager pour accéder au compte dans le service Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "mot de passe");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### Voir également

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* espace de noms [Aspose.Tasks](../../projectservermanager/)
* Assemblée [Aspose.Tasks](../../../)


