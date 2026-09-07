---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta una password utilizzata per proteggere il file MPP risultante. Attualmente è supportato per i formati MS Project 2010 e successivi. Un valore null indica che il file di progetto non è protetto."
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Ottiene o imposta una password utilizzata per proteggere il file MPP risultante. Attualmente è supportata per i formati MS Project 2010 e versioni successive. Un valore null indica che il file di progetto non è protetto.

```csharp
public string ProtectionPassword { get; set; }
```

## Esempi

Mostra come salvare un progetto in un file MPP protetto da password.

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

### Vedi anche

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


