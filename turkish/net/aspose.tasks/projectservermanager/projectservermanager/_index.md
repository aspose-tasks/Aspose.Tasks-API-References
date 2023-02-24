---
title: ProjectServerManager.ProjectServerManager
second_title: Aspose.Tasks for .NET API Referansı
description: ProjectServerManager inşaatçı. Yeni bir örneğini başlatır.ProjectServerManager sınıf.
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Yeni bir örneğini başlatır.[`ProjectServerManager`](../) sınıf.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Project Online hesabına bağlanmak için kullanılan kimlik bilgileri. |

### Örnekler

Bu örnek, Project Server'ın şirket içi örneğine erişmek için ProjectServerManager örneğinin nasıl oluşturulacağını gösterir.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Bu örnek, Project Online hizmetinde hesaba erişmek için ProjectServerManager örneğinin nasıl oluşturulacağını gösterir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "şifre");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

### Ayrıca bakınız

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* ad alanı [Aspose.Tasks](../../projectservermanager/)
* toplantı [Aspose.Tasks](../../../)


