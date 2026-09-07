---
title: "Απαρίθμηση RateScaleType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.RateScaleType. Καθορίζει τον τύπο κλίμακας ρυθμού"
type: docs
weight: 1650
url: /el/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Καθορίζει τον τύπο κλίμακας ρυθμού.

```csharp
public enum RateScaleType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `0` | Δείχνει ακαθόριστο τύπο κλίμακας ρυθμού. |
| Minute | `1` | Δείχνει τύπο κλίμακας ρυθμού Λεπτό. |
| Hour | `2` | Δείχνει τύπο κλίμακας ρυθμού Ώρα. |
| Day | `3` | Δείχνει τύπο κλίμακας ρυθμού Ημέρα. |
| Week | `4` | Δείχνει τύπο κλίμακας ρυθμού Εβδομάδα. |
| Month | `5` | Δείχνει τύπο κλίμακας ρυθμού Μήνας. |
| Quarter | `6` | Δείχνει τύπο κλίμακας ρυθμού Τρίμηνο. |
| Year | `7` | Δείχνει τύπο κλίμακας ρυθμού Έτος. |

## Παραδείγματα

Δείχνει πώς να ορίσετε μεταβλητή κατανάλωση υλικού (π.χ. '10/ημέρα' ή '1/εβδομάδα') για μια ανάθεση υλικού πόρου.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Ας υποθέσουμε ότι θέλουμε να ορίσουμε κατανάλωση υλικού '1/εβδομάδα'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

Δείχνει πώς να εργαστείτε με την κλίμακα ρυθμού της ανάθεσης όταν θέλουμε να ορίσουμε μεταβλητή κατανάλωση υλικού (π.χ. '10/ημέρα' ή '1/εβδομάδα') για μια ανάθεση υλικού πόρου.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Ας υποθέσουμε ότι θέλουμε να ορίσουμε κατανάλωση υλικού '1/εβδομάδα'.
// Πρέπει να ορίσουμε την ωριαία τιμή στην ιδιότητα Units, ώστε να διαιρέσουμε 1D με τις ώρες ανά εβδομάδα.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Παρακαλώ σημειώστε ότι από την έκδοση 24.4 και μετά αυτό μπορεί να γίνει καλώντας 1 μέθοδο:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Μόνο οι αναθέσεις υλικού πόρου μπορούν να έχουν μη μηδενική τιμή κλίμακας ρυθμού.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


