---
title: "Klasse InvalidPasswordException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.InvalidPasswordException klasse. Vertegenwoordigt het type uitzondering dat wordt gegooid bij het openen van een met wachtwoord beveiligd bestand met een verkeerd wachtwoord"
type: docs
weight: 910
url: /nl/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Stelt het type uitzondering voor dat wordt gegooid wanneer een met wachtwoord beschermd bestand wordt geopend met een verkeerd wachtwoord.

```csharp
public class InvalidPasswordException : TasksException
```

## Voorbeelden

Toont hoe &lt;see cref=\"InvalidPasswordException\"/&gt; te behandelen tijdens het lezen van wachtwoordbeveiligde projectbestanden.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // werken met project ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // het bericht is \"Het project is wachtwoordbeveiligd. Het wachtwoord is niet opgegeven of onjuist.\"
    Console.WriteLine(e.Message);
}
```

### Zie ook

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


