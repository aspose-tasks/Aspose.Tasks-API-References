---
title: "Classe OleObject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.OleObject classe. Rappresenta un oggetto OLE che può essere inserito nella visualizzazione Gantt Chart di un file MPP"
type: docs
weight: 1120
url: /it/net/aspose.tasks/oleobject/
---
## OleObject class

Rappresenta un oggetto OLE che può essere inserito nella vista Gantt Chart di un file MPP.

```csharp
public class OleObject
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OleObject](oleobject/)() | Inizializza una nuova istanza della classe `OleObject`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Ottiene o imposta il nome dell'applicazione con cui aprire l'oggetto incorporato. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Ottiene o imposta i dati del file incorporato; null se non sono stati incorporati dati. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Ottiene o imposta un flag che indica se l'oggetto OLE deve essere mostrato come icona o come immagine normale. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Ottiene o imposta il formato file dell'oggetto incorporato. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Ottiene o imposta il percorso completo dell'oggetto inserito. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Ottiene o imposta l'ID dell'oggetto. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Ottiene o imposta l'etichetta dell'oggetto inserito. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Ottiene un valore che indica se il file di progetto contiene solo un collegamento ai dati effettivi memorizzati nella sorgente del collegamento. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Ottiene o imposta il nome dell'istanza dell'oggetto OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Ottiene o imposta il percorso al file temporaneo dell'oggetto inserito. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Ottiene o imposta l'istanza della classe [`View`](./view/) a cui appartiene l'oggetto inserito. |

## Esempi

Mostra come leggere le informazioni sugli oggetti OLE.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


