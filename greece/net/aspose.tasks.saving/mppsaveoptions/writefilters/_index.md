---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα φίλτρων κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα φίλτρων περιλαμβάνουν τις συλλογές Project.TaskFilters και Project.ResourceFilters."
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα φίλτρων κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα φίλτρων περιλαμβάνουν τις συλλογές Project.TaskFilters και Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Παρατηρήσεις

Αυτή τη στιγμή υποστηρίζεται για μορφές MSP 2010 ή νεότερες.

## Παραδείγματα

Δείχνει πώς να προσθέσετε και να αποθηκεύσετε νέο φίλτρο εργασιών σε έργο MPP.

```csharp
Project project = new Project();

project.TaskFilters.Clear();
project.ResourceFilters.Clear();

var filter = new Filter();
filter.Name = "New Task Filter";
filter.FilterType = ItemType.TaskItem;
filter.ShowInMenu = true;
filter.ShowRelatedSummaryRows = true;

filter.Criteria = new FilterCriteria();

var criteria1 = new FilterCriteria();
criteria1.Field = Field.TaskNumber13;
criteria1.Test = FilterComparisonType.IsLessThan;
criteria1.Values[0] = 34.3D;

filter.Criteria.CriteriaRows.Add(criteria1);
project.TaskFilters.Add(filter);

SimpleSaveOptions options = new MPPSaveOptions() { WriteFilters = true };
project.Save(OutDir + "output_new_filter.mpp", options);
```

### Δείτε επίσης

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


