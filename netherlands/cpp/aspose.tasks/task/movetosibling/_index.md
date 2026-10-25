---
title: "Aspose::Tasks::Task::MoveToSibling methode"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks voor C++"
description: "Verplaatst de huidige taak op hetzelfde outline-niveau vóór de opgegeven taak."
type: docs
weight: 1370
url: /nl/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Verplaatst de huidige taak op hetzelfde Outline-niveau vóór de opgegeven taak. Als ParentProject.CalculationMode None is, moet de gebruiker na het gebruik van deze methode Project.Recalculate() aanroepen (dit zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden zoals slack, werk- en kostengebieden, outline-niveaus berekenen). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak‑ID, outline‑niveau en outline‑nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start-/einddatums, stelt vroege/late datums in, berekent slack, werk‑ en kostengebieden, herberekent ID’s en outline‑niveaus).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parameter | Beschrijving |
| --- | --- |
| beforeTask | Taak vóór welke de huidige taak wordt ingevoegd. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Verplaatst de huidige taak op hetzelfde outline-niveau vóór een taak met de opgegeven Id. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (deze zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen, zoals speling, werk‑ en kostengebieden, outline‑niveaus). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak‑id, outline‑niveau en outline‑nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start-/einddatums, stelt vroege/late datums in, berekent speling, werk‑ en kostengebieden, recalculates ids en outline‑niveaus).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parameter | Beschrijving |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) van een taak vóór welke de huidige taak wordt ingevoegd. |

