---
title: "Enum ApplicationInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.ApplicationInfo enum. Specifica la versione del progetto in cui è stato creato il file"
type: docs
weight: 10
url: /it/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Specifica la versione del progetto in cui è stato creato il file.

```csharp
public enum ApplicationInfo
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `0` | Non può essere definito. |
| MSP2000 | `1` | Il file è stato creato in Microsoft Project 2000/2002. |
| MSP2003 | `2` | Il file è stato creato in Microsoft Project 2003. |
| MSP2007 | `3` | Il file è stato creato in Microsoft Project 2007. |
| MSP2010 | `4` | Il file è stato creato in Microsoft Project 2010. |
| MSP2013 | `5` | Il file è stato creato in Microsoft Project 2013. |
| MSP2016 | `6` | Il file è stato creato in Microsoft Project 2016. |

## Esempi

Mostra come verificare le informazioni sull'applicazione del progetto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


