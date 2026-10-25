---
title: "Enum FileFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.FileFormat enum. Specifica il formato file dei progetti"
type: docs
weight: 590
url: /it/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Specifica il formato file del progetto.

```csharp
public enum FileFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `0` | Non può essere definito. |
| P6XML | `1` | Rappresenta il formato XML di Primavera P6. |
| XML | `2` | Formato XML di Microsoft Project. |
| MPP8 | `3` | Formato Microsoft Project 2000. |
| MPP9 | `4` | Formato Microsoft Project 2003. |
| MPP12 | `5` | Formato Microsoft Project 2007. |
| MPP14 | `6` | Formato Microsoft Project 2010. |
| MPT9 | `7` | Formato modello Microsoft Project 2003. |
| MPT12 | `8` | Formato modello Microsoft Project 2007. |
| MPT14 | `9` | Formato modello Microsoft Project 2010 (2013). |
| MPX | `10` | Formato file Mpx |
| XER | `11` | Rappresenta il formato Primavera XER |
| HTML | `12` | Rappresenta il formato HTML |
| ProjectServer | `13` | Il progetto è stato letto da Project Server o Project Online |

## Esempi

Mostra come leggere il formato del file di verifica del progetto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


