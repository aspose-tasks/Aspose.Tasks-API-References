---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Γεγονός ProjectServerManager. Ένα γεγονός που ενεργοποιείται όταν το αίτημα ιστού αποστέλλεται στο web API του Project Server."
type: docs
weight: 20
url: /el/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Ένα συμβάν που ενεργοποιείται όταν το web request αποστέλλεται στο web API του Project Server.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το γεγονός ProjectServerManager.ExecutingWebRequest για να προσαρμόσετε τα αιτήματα ιστού που αποστέλλονται στο Project Server.

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

### Δείτε επίσης

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


