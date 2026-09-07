---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ResourceAssignment-Methode. Legt Einheiten für die Zuweisung einer materiellen Ressource mit variablem Materialverbrauch fest. Der variable Materialverbrauch bedeutet, dass sich die Menge der verwendeten Materialien proportional ändert, wenn die Zuweisungsdauer sich ändert."
type: docs
weight: 760
url: /de/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Legt Einheiten für die Zuweisung einer materiellen Ressource mit variablem Materialverbrauch fest. Der variable Materialverbrauch bedeutet, dass sich die Menge der verwendeten Materialien proportional ändert, wenn die Zuweisungsdauer sich ändert.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Einheiten | Double | Anzahl der im Zeitraum angesammelten Einheiten. |
| rateScaleType | RateScaleType | Zeitraum, in dem der Einheitswert angesammelt wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| InvalidOperationException | Wenn die Methode für die Zuweisung einer nicht-materiellen Ressource aufgerufen wird. |

## Hinweise

Zum Beispiel sollte zum Setzen von '123/Monat' SetUnitsScaled(123D, RateScaleType.Month) aufgerufen werden.

## Beispiele

Zeigt, wie man variablen Materialverbrauch (z. B. '10/Tag' oder '1/Woche') für die Zuweisung einer materiellen Ressource festlegt.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Angenommen, wir wollen den Materialverbrauch auf '1/Woche' setzen.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### Siehe auch

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


