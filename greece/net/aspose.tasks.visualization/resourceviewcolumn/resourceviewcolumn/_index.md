---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ResourceViewColumn. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης ResourceViewColumn"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| μετατροπέας | ResourceToColumnTextConverter | Μετατροπέας δεδομένων πόρου σε κείμενο στήλης. |
| πεδίο | Πεδίο | Πεδίο στήλης. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής πόρων για εξαγωγή.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// επανάληψη στις στήλες
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Δείτε επίσης

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα στήλης. |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| μετατροπέας | ResourceToColumnTextConverter | Μετατροπέας δεδομένων πόρου σε κείμενο στήλης. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής πόρων για εξαγωγή.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// επανάληψη στις στήλες
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Δείτε επίσης

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(int width, Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πλάτος | Int32 | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | Πεδίο | Πεδίο στήλης. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής πόρων για εξαγωγή.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// επανάληψη στις στήλες
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Δείτε επίσης

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


