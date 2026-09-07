---
title: "Table.TableFields"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Table. Ottiene una raccolta TableFields che rappresenta i campi nella tabella"
type: docs
weight: 90
url: /it/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Ottiene una collezione TableFields che rappresenta i campi nella tabella.

```csharp
public TableFieldCollection TableFields { get; }
```

## Esempi

Mostra come gestire le tabelle del progetto.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Definisci un nuovo attributo personalizzato
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Aggiungi un attributo di testo personalizzato al task creato.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Personalizza la tabella aggiungendo il campo attributo di testo
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

### Vedi anche

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


