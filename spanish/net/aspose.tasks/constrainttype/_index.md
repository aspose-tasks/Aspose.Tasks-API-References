---
title: "Enumeración ConstraintType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.ConstraintType. Especifica la restricción sobre la fecha de inicio o fin de una tarea"
type: docs
weight: 330
url: /es/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Especifica la restricción sobre la fecha de inicio o fin de una tarea.

```csharp
public enum ConstraintType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | El valor no estaba definido en el archivo de proyecto original. |
| AsSoonAsPossible | `0` | Las fechas [`Start`](../tsk/start/) y [`Finish`](../tsk/finish/) de [`Task`](../task/) se programan lo antes posible con respecto a las fechas padre [`Start`](../tsk/start/) y [`Finish`](../tsk/finish/) y considerando los [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | Las fechas de [`Start`](../tsk/start/) y [`Finish`](../tsk/finish/) de [`Task`](../task/) se programan ALAP con respecto a las fechas de inicio y fin del padre y considerando [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Debe iniciar el |
| MustFinishOn | `3` | Debe finalizar el |
| StartNoEarlierThan | `4` | Inicio no antes de |
| StartNoLaterThan | `5` | Inicio no después de |
| FinishNoEarlierThan | `6` | Fin no antes de |
| FinishNoLaterThan | `7` | Fin no después de |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo establecer la restricción &lt;see cref="Aspose.Tasks.ConstraintType" /&gt; ConstraintType.AsSoonAsPossible para una tarea.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Establecer la restricción As Soon As Possible para la tarea con Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


