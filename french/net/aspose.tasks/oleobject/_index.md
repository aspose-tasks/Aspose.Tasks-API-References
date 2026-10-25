---
title: "Classe OleObject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OleObject. Représente un objet OLE qui peut être inséré dans la vue du diagramme de Gantt d'un fichier MPP"
type: docs
weight: 1120
url: /fr/net/aspose.tasks/oleobject/
---
## OleObject class

Représente un objet OLE qui peut être inséré dans la vue Gantt Chart d'un fichier MPP.

```csharp
public class OleObject
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OleObject](oleobject/)() | Initialise une nouvelle instance de la classe `OleObject`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Obtient ou définit le nom de l'application avec laquelle ouvrir l'objet intégré. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Obtient ou définit les données du fichier intégré ; null si aucune donnée n'a été intégrée. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Obtient ou définit un indicateur indiquant que l'objet OLE doit être affiché soit sous forme d'icône, soit sous forme d'image normale. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Obtient ou définit le format de fichier de l'objet intégré. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Obtient ou définit le chemin complet de l'objet inséré. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Obtient ou définit l'identifiant de l'objet. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Obtient ou définit le libellé de l'objet inséré. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Obtient une valeur indiquant si le fichier de projet ne contient qu'un lien vers les données réelles stockées à la source du lien. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Obtient ou définit le nom de l'instance de l'objet OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Obtient ou définit le chemin du fichier temporaire de l'objet inséré. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Obtient ou définit l'instance de la classe [`View`](./view/) à laquelle appartient l'objet inséré. |

## Exemples

Montre comment lire les informations sur les objets OLE.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


