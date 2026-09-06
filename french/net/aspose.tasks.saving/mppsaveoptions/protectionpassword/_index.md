---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit un mot de passe utilisé pour protéger le fichier MPP résultant. Actuellement pris en charge pour les formats MS Project 2010 et plus récents. Une valeur null indique que le fichier projet n'est pas protégé."
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Obtient ou définit un mot de passe utilisé pour protéger le fichier MPP résultant. Actuellement, il est pris en charge pour les formats MS Project 2010 et ultérieurs. Une valeur null indique que le fichier de projet n'est pas protégé.

```csharp
public string ProtectionPassword { get; set; }
```

## Exemples

Montre comment enregistrer un projet dans un fichier MPP protégé par mot de passe.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### Voir aussi

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


