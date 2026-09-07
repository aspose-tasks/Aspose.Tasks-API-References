---
title: "Project.SetBaseline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Αποθηκεύει τα πεδία baseline στο καθορισμένο baseline για ολόκληρο το έργο"
type: docs
weight: 1250
url: /el/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Αποθηκεύει τα πεδία baseline στο καθορισμένο baseline για ολόκληρο το έργο.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| baselineType | BaselineType | Ο τύπος baseline για την αποθήκευση των δεδομένων baseline. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε baselines για ολόκληρο το έργο.

```csharp
var project = new Project();

// Προσθήκη εργασιών
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Ορισμός baseline για καθορισμένες εργασίες
project.SetBaseline(BaselineType.Baseline);
```

### Δείτε επίσης

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Αποθηκεύει τα πεδία baseline στο καθορισμένο baseline για τις επιλεγμένες εργασίες.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| baselineType | BaselineType | Ο τύπος baseline για την αποθήκευση των δεδομένων baseline. |
| taskCollection | IEnumerable`1 | Λίστα εργασιών για τις οποίες θα αποθηκευτούν δεδομένα baseline. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε baselines για συγκεκριμένες εργασίες.

```csharp
var project = new Project();

// Προσθήκη εργασιών
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Ορισμός baseline για καθορισμένες εργασίες
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Δείτε επίσης

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


