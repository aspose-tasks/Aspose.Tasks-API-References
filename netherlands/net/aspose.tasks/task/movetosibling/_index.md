---
title: MoveToSibling
second_title: Aspose.Tasks voor .NET API-referentie
description: Verplaatst de huidige taak naar hetzelfde overzichtsniveau vóór de opgegeven taak. Als ParentProject.CalculationMode Geen is moet de gebruiker Project.Recalculate aanroepen na gebruik van deze methode het zal alle projecttaken opnieuw plannen start/einddatums late datums en bereken de afhankelijke velden zoals speling werk en kostenvelden overzichtsniveaus. Als ParentProject.CalculationMode Handmatig is berekent de methode alleen taakID overzichtsniveau en overzichtsnummers automatisch. Als ParentProject.CalculationMode Automatisch is de methode plant automatisch alle projecttaken opnieuw begin/einddatums stelt vroege/late datums in berekent speling werk en kostenvelden herberekent ids en overzichtsniveaus.
type: docs
weight: 1370
url: /nl/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Verplaatst de huidige taak naar hetzelfde overzichtsniveau vóór de opgegeven taak. Als ParentProject.CalculationMode Geen is, moet de gebruiker Project.Recalculate() aanroepen na gebruik van deze methode (het zal alle projecttaken opnieuw plannen (start-/einddatums, late datums) en bereken de afhankelijke velden zoals speling, werk- en kostenvelden, overzichtsniveaus). Als ParentProject.CalculationMode Handmatig is, berekent de methode alleen taak-ID, overzichtsniveau en overzichtsnummers automatisch. Als ParentProject.CalculationMode Automatisch is de methode plant automatisch alle projecttaken opnieuw (begin-/einddatums, stelt vroege/late datums in, berekent speling, werk- en kostenvelden, herberekent id's en overzichtsniveaus).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beforeTask | Task | Taak waarvoor de huidige taak wordt ingevoegd. |

### Zie ook

* class [Task](../)
* naamruimte [Aspose.Tasks](../../task/)
* montage [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Verplaatst de huidige taak naar hetzelfde overzichtsniveau vóór een taak met de opgegeven id. Als ParentProject.CalculationMode Geen is, moet de gebruiker Project.Recalculate() aanroepen na gebruik van deze methode (het zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en berekent de afhankelijke velden zoals speling, werk- en kostenvelden, overzichtsniveaus). Als ParentProject.CalculationMode Handmatig is, berekent de methode alleen taak-ID, overzichtsniveau en overzichtsnummers automatisch. Als ParentProject. CalculationMode is automatisch, de methode plant alle projecttaken automatisch opnieuw (begin-/einddatums, stelt vroege/late datums in, berekent speling, werk- en kostenvelden, herberekent id's en overzichtsniveaus).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beforeTaskId | Int32 | ID kaart ([`Id`](../../tsk/id/)) van een taak waarvoor de huidige taak wordt ingevoegd. |

### Zie ook

* class [Task](../)
* naamruimte [Aspose.Tasks](../../task/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->