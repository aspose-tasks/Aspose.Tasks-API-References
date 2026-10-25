---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Event ProjectServerManager. Sebuah event yang dipicu ketika permintaan web dikirim ke API web Project Server."
type: docs
weight: 20
url: /id/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Sebuah peristiwa yang dipicu ketika permintaan web dikirim ke API web Project Server.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Contoh

Menampilkan cara menggunakan event ProjectServerManager.ExecutingWebRequest untuk menyesuaikan permintaan web yang dikirim ke Project Server.

```csharp
try
{
    const string SiteUrl = "https://myprojectserver/sites/pwa";
    const string UserName = "test_user";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SiteUrl, new NetworkCredential(UserName, Password));

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.ExecutingWebRequest += delegate (object sender, WebRequestEventArgs e)
    {
        e.WebRequest.Headers.Add("XMyCustomHeader", "testvalue");
    };

    var list = manager.GetProjectList();
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


