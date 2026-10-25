---
title: "Asn.RateScale"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Asn field. Η μονάδα χρόνου για το ρυθμό χρήσης της ανάθεσης υλικού πόρου. Επιστρέφει 0 εάν δεν ορίζεται"
type: docs
weight: 410
url: /el/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

Η μονάδα χρόνου για το ρυθμό χρήσης της υλικής ανάθεσης πόρου. Επιστρέφει 0 εάν δεν ορίζεται.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Παραδείγματα

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


