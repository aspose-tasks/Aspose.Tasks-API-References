---
title: "Classe PrimaveraXmlReader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.PrimaveraXmlReader. Rappresenta un lettore che consente di recuperare gli UID del progetto da un file XML Primavera"
type: docs
weight: 1400
url: /it/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Rappresenta un lettore che consente di recuperare gli UID del progetto da un file Primavera Xml.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Inizializza una nuova istanza della classe `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Inizializza una nuova istanza della classe `PrimaveraXmlReader`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Restituisce un elenco degli oggetti di informazioni brevi del progetto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Restituisci un elenco degli identificatori univoci dei progetti. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Carica il progetto con l'identificatore univoco specificato. |

## Esempi

Mostra come esaminare le informazioni di progetti brevi da un file XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Vedi anche

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


