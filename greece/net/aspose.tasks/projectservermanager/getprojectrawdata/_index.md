---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectServerManager. Λαμβάνει τα δυαδικά δεδομένα του έργου για σκοπούς αντιμετώπισης προβλημάτων."
type: docs
weight: 60
url: /el/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Αποκτά τα δυαδικά δεδομένα του έργου για σκοπούς αντιμετώπισης προβλημάτων.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectGuid | Guid | Το Guid του έργου που θα διαβαστεί. |

### Τιμή Επιστροφής

Ροή που περιέχει τα ακατέργαστα δεδομένα του έργου.

## Παραδείγματα

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid του έργου που προσπαθείτε να λάβετε.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

Δείχνει πώς να ανακτήσετε τα ακατέργαστα δεδομένα του έργου από το Microsoft Project Online για σκοπούς αντιμετώπισης προβλημάτων.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // Ο χρήστης μπορεί να διαβάσει το έργο ως ροή ακατέργαστων δεδομένων για σκοπούς αντιμετώπισης προβλημάτων.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // Μπορείτε να περάσετε το παραγόμενο αρχείο στην υποστήριξη.
}
```

### Δείτε επίσης

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


