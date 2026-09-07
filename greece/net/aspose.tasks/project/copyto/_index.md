---
title: "Project.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Project method. Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε άλλο έργο"
type: docs
weight: 1060
url: /el/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε άλλο έργο.

```csharp
public void CopyTo(Project another)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | Project | Άλλο έργο για αντιγραφή δεδομένων. |

## Παραδείγματα

Δείχνει πώς να αντιγράψετε τα δεδομένα του έργου σε άλλο έργο.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// παραλείψτε την αντιγραφή των δεδομένων προβολής κατά την αντιγραφή κοινών δεδομένων έργου.
project.CopyTo(mppProject);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Αντιγράφει τα κύρια δεδομένα και τις ιδιότητες του έργου σε άλλο έργο.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | Project | Άλλο έργο για αντιγραφή δεδομένων. |
| επιλογές | CopyToOptions | Επιλογές αντιγραφής για έλεγχο της διαδικασίας αντιγραφής. |

## Παραδείγματα

Δείχνει πώς να αντιγράψετε το έργο με χρήση του αντικειμένου &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// παραλείψτε την αντιγραφή των δεδομένων προβολής κατά την αντιγραφή κοινών δεδομένων έργου.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Δείτε επίσης

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


