---
title: "Κλάση OleObjectCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.OleObjectCollection κλάση. Αντιπροσωπεύει μια συλλογή που περιέχει τις εμφανίσεις της κλάσης OleObject"
type: docs
weight: 1130
url: /el/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Αντιπροσωπεύει μια συλλογή που περιέχει τις εμφανίσεις της κλάσης [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Καθαρίζει τη συλλογή. Για να διατηρηθούν αυτές οι αλλαγές, πρέπει να κληθεί το project.Save με νέο MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Μετατρέπει την παρουσία της κλάσης `OleObjectCollection` σε λίστα που περιέχει τις εμφανίσεις της κλάσης [`OleObject`](../oleobject/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογή αντικειμένων OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// χρησιμοποιώντας πρόσβαση με δείκτη
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// or enumeration one can iterate over OLE objects
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### Δείτε επίσης

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


