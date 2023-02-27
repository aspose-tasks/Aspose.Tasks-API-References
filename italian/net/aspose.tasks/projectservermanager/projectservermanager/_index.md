---
title: ProjectServerManager.ProjectServerManager
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ProjectServerManager costruttore. Inizializza una nuova istanza diProjectServerManager classe.
type: docs
weight: 10
url: /it/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Inizializza una nuova istanza di[`ProjectServerManager`](../) classe.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Credenziali usate per connettersi all'account di Project online. |

### Esempi

Questo esempio mostra come creare un'istanza di ProjectServerManager per accedere all'istanza locale di Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Questo esempio mostra come creare un'istanza di ProjectServerManager per accedere all'account nel servizio Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### Guarda anche

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* spazio dei nomi [Aspose.Tasks](../../projectservermanager/)
* assemblea [Aspose.Tasks](../../../)


