---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Ορίζει μονάδες για την ανάθεση ενός υλικού πόρου με μεταβλητή κατανάλωση υλικού. Η μεταβλητή κατανάλωση υλικού σημαίνει ότι καθώς αλλάζει η διάρκεια της ανάθεσης, η ποσότητα των χρησιμοποιούμενων υλικών αλλάζει αναλογικά."
type: docs
weight: 760
url: /el/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Ορίζει μονάδες για την ανάθεση ενός υλικού πόρου με μεταβλητή κατανάλωση υλικού. Η μεταβλητή κατανάλωση υλικού σημαίνει ότι καθώς αλλάζει η διάρκεια της ανάθεσης, η ποσότητα των χρησιμοποιούμενων υλικών αλλάζει αναλογικά.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μονάδες | Double | Αριθμός μονάδων που συσσωρεύονται στην χρονική περίοδο. |
| rateScaleType | RateScaleType | Χρονική περίοδος κατά την οποία η τιμή της μονάδας συσσωρεύεται. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν η μέθοδος κληθεί για ανάθεση μη υλικού πόρου. |

## Παρατηρήσεις

Για παράδειγμα, για να ορίσετε '123/μήνα', πρέπει να κληθεί η SetUnitsScaled(123D, RateScaleType.Month).

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

### Δείτε επίσης

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


