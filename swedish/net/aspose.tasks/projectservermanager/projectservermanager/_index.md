---
title: ProjectServerManager.ProjectServerManager
second_title: Aspose.Tasks för .NET API-referens
description: ProjectServerManager byggare. Initierar en ny instans avProjectServerManager class.
type: docs
weight: 10
url: /sv/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Initierar en ny instans av[`ProjectServerManager`](../) class.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Inloggningsuppgifter som används för att ansluta till Project Online-konto. |

### Exempel

Det här exemplet visar hur man skapar en instans av ProjectServerManager för att komma åt den lokala instansen av Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Det här exemplet visar hur man skapar en instans av ProjectServerManager för att komma åt kontot i Project Online-tjänsten.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxxx.onmicrosoft.com", "lösenord");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### Se även

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namnutrymme [Aspose.Tasks](../../projectservermanager/)
* hopsättning [Aspose.Tasks](../../../)


