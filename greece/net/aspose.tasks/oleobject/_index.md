---
title: "Κλάση OleObject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.OleObject κλάση. Αντιπροσωπεύει ένα αντικείμενο OLE που μπορεί να εισαχθεί στην προβολή Gantt Chart ενός αρχείου MPP"
type: docs
weight: 1120
url: /el/net/aspose.tasks/oleobject/
---
## OleObject class

Αντιπροσωπεύει ένα αντικείμενο OLE που μπορεί να εισαχθεί στην προβολή Gantt Chart ενός αρχείου MPP.

```csharp
public class OleObject
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [OleObject](oleobject/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `OleObject`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της εφαρμογής με την οποία θα ανοίξει το ενσωματωμένο αντικείμενο. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Λαμβάνει ή ορίζει τα δεδομένα του ενσωματωμένου αρχείου· null εάν δεν ενσωματώθηκαν δεδομένα. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Λαμβάνει ή ορίζει μια σημαία που υποδεικνύει ότι το αντικείμενο OLE πρέπει να εμφανίζεται είτε ως εικονίδιο είτε ως κανονική του εικόνα. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή αρχείου του ενσωματωμένου αντικειμένου. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Λαμβάνει ή ορίζει τη πλήρη διαδρομή του εισαχθέντος αντικειμένου. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Λαμβάνει ή ορίζει το αναγνωριστικό (id) του αντικειμένου. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Λαμβάνει ή ορίζει την ετικέτα του εισαχθέντος αντικειμένου. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το αρχείο έργου περιέχει μόνο έναν σύνδεσμο προς τα πραγματικά δεδομένα που αποθηκεύονται στην πηγή του συνδέσμου. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της παρουσίασης του αντικειμένου OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Λαμβάνει ή ορίζει τη διαδρομή προς το προσωρινό αρχείο του εισαχθέντος αντικειμένου. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Λαμβάνει ή ορίζει την παρουσία της κλάσης [`View`](./view/) στην οποία ανήκει το εισαχθέν αντικείμενο. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες σχετικά με τα αντικείμενα OLE.

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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


