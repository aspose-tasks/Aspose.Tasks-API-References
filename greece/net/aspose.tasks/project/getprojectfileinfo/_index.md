---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Διαβάζει τις πληροφορίες αρχείου του έργου από το αρχείο"
type: docs
weight: 1280
url: /el/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Διαβάζει πληροφορίες αρχείου έργου από το αρχείο.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα αρχείου | String | Το όνομα αρχείου του έργου. |

### Τιμή Επιστροφής

Οι πληροφορίες αρχείου του έργου [`ProjectFileInfo`](../../projectfileinfo/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πληροφορίες αρχείου του έργου που διαβάστηκαν από ένα αρχείο XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Λαμβάνει πληροφορίες αρχείου έργου από τη ροή.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Η ροή δεδομένων. |

### Τιμή Επιστροφής

Οι πληροφορίες αρχείου του έργου [`ProjectFileInfo`](../../projectfileinfo/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες αρχείου έργου ενός αρχείου XML που διαβάζεται από ροή.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Δείτε επίσης

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


