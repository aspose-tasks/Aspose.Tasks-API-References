---
title: "Classe LoadOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.LoadOptions. Consente di specificare parametri di caricamento aggiuntivi quando si carica un progetto da file o stream"
type: docs
weight: 990
url: /it/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Consente di specificare parametri di caricamento aggiuntivi quando si carica un progetto da file o stream.

```csharp
public class LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LoadOptions](loadoptions/)() | Inizializza una nuova istanza della classe `LoadOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Ottiene o imposta un token che può essere usato per annullare un'operazione di caricamento del progetto. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Ottiene o imposta la codifica utilizzata per leggere un progetto da formati HTML, MPX, XER e Primavera XML. La codifica predefinita è UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Ottiene o imposta un metodo di callback per gestire gli errori di parsing XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Ottiene o imposta una password di protezione. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Ottiene o imposta un'istanza specificata della classe [`PrimaveraReadOptions`](../primaverareadoptions/) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Ottiene o imposta il callback da invocare durante le operazioni di caricamento del progetto. Attualmente supportato per i formati MPP e XER. |

## Esempi

Mostra come caricare il progetto protetto da password usando l'istanza &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


