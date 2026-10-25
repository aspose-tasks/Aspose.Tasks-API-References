---
title: "Klasse OleObject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OleObject class. Vertegenwoordigt een OLE-object dat kan worden ingevoegd in de Gantt-diagramweergave van een MPP-bestand"
type: docs
weight: 1120
url: /nl/net/aspose.tasks/oleobject/
---
## OleObject class

Stelt een OLE‑object voor dat kan worden ingevoegd in de Gantt Chart‑weergave van een MPP‑bestand.

```csharp
public class OleObject
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [OleObject](oleobject/)() | Initialiseert een nieuw exemplaar van de `OleObject`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Haalt op of stelt de toepassingsnaam in waarmee het ingebedde object wordt geopend. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Haalt op of stelt de gegevens van het ingebedde bestand in; null als er geen gegevens zijn ingebed. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Haalt op of stelt een vlag in die aangeeft dat het OLE-object moet worden weergegeven als een pictogram of als de reguliere afbeelding. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Haalt op of stelt het bestandsformaat van het ingebedde object in. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Haalt op of stelt het volledige pad van het ingevoegde object in. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Haalt op of stelt de object-id in. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Haalt op of stelt het label van het ingevoegde object in. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Haalt een waarde op die aangeeft of het projectbestand alleen een koppeling bevat naar de daadwerkelijke gegevens die bij de koppelingsbron zijn opgeslagen. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Haalt op of stelt de naam van de instantie van het OLE-object in. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Haalt op of stelt het pad naar het tijdelijke bestand van het ingevoegde object in. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Haalt op of stelt de instantie van de [`View`](./view/)-klasse in waartoe het ingevoegde object behoort. |

## Voorbeelden

Toont hoe informatie over OLE-objecten kan worden gelezen.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


