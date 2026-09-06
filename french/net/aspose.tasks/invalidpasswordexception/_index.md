---
title: "Classe InvalidPasswordException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.InvalidPasswordException. Représente le type d'exception qui est levé lors de l'ouverture d'un fichier protégé par mot de passe avec un mot de passe incorrect."
type: docs
weight: 910
url: /fr/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Représente le type d'exception qui est levé lors de l'ouverture d'un fichier protégé par mot de passe avec un mot de passe incorrect.

```csharp
public class InvalidPasswordException : TasksException
```

## Exemples

Montre comment gérer &lt;see cref=\"InvalidPasswordException\"/&gt; lors de la lecture de fichiers de projet protégés par mot de passe.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // travail avec le projet ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // le message est \"Le projet est protégé par mot de passe. Le mot de passe n'est pas fourni ou est incorrect.\"
    Console.WriteLine(e.Message);
}
```

### Voir aussi

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


