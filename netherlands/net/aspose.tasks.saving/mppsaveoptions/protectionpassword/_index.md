---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een wachtwoord op of stelt dit in dat wordt gebruikt om een resulterend MPP‑bestand te beveiligen. Momenteel ondersteund voor MS Project 2010 en nieuwere formaten. Een null‑waarde geeft aan dat het projectbestand niet beveiligd is."
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Haalt op of stelt een wachtwoord in dat wordt gebruikt om een resulterend MPP‑bestand te beveiligen. Momenteel wordt dit ondersteund voor MS Project 2010 en nieuwere formaten. Een null‑waarde geeft aan dat het projectbestand niet beveiligd is.

```csharp
public string ProtectionPassword { get; set; }
```

## Voorbeelden

Toont hoe een project op te slaan naar een met wachtwoord beveiligd MPP‑bestand.

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

### Zie ook

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


