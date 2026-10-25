---
title: "Table.TableFields"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Table property. Haalt een TableFields-collectie op die de velden in de tabel weergeeft"
type: docs
weight: 90
url: /nl/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Haalt een TableFields-collectie op die de velden in de tabel vertegenwoordigt.

```csharp
public TableFieldCollection TableFields { get; }
```

## Voorbeelden

Toont hoe je met de tabellen van een project werkt.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Definieer een nieuw aangepast attribuut
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Voeg een aangepast tekstattribuut toe aan de aangemaakte taak.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Pas de tabel aan door een tekstattribuutveld toe te voegen
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Zie ook

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


