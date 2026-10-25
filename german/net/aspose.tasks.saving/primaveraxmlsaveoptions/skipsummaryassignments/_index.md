---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "PrimaveraXmlSaveOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob Zuordnungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen."
type: docs
weight: 30
url: /de/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Gibt einen Wert zurück oder legt ihn fest, der angibt, ob Zuordnungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Hinweise

Die Primavera-Software unterstützt keine Zuordnungen von Ressourcen zu Zusammenfassungs- (WBS-) Aufgaben. Daher kann der Export solcher Zuordnungen zu einer ungültigen Datei führen, die nicht dem Primavera-Model entspricht. Ist der Wert true, werden Zuordnungen zu Zusammenfassungsaufgaben beim Export übersprungen. Ist er false (der Standardwert), wird eine Ausnahme ausgelöst, wenn beim Export eine Zuordnung zu einer Zusammenfassungsaufgabe gefunden wird.

## Beispiele

Zeigt, wie das Flag SkipSummaryAssignments verwendet wird.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera unterstützt keine Zuordnungen von Ressourcen zu Zusammenfassungsaufgaben.
// Das Exportieren solcher Zuordnungen in das Primavera-Format kann daher zu Dateien führen, die nicht in Primavera importiert werden können.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Siehe auch

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


