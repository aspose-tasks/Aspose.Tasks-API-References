---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete method"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks voor C++"
description: "Werk alle werkzaamheden bij als voltooid tot een opgegeven datum voor het gehele project."
type: docs
weight: 2080
url: /nl/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Werk alle werkzaamheden bij als voltooid tot een opgegeven datum voor het gehele project.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Beschrijving |
| --- | --- |
| completeThrough | De datum om het werk bij te werken tot voltooid. |
| setZeroOrHundredPercentCompleteOnly | Indien ingesteld op true, werkt alleen die taken bij als 100% voltooid waarvan de einddatum vóór de opgegeven voltooid‑tot datum ligt. Anders wordt een voltooiingspercentage berekend op basis van de geplande start‑ en voltooid‑tot datums. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Werkt al het werk bij als voltooid tot een opgegeven datum voor de opgegeven lijst met taken.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parameter | Beschrijving |
| --- | --- |
| completeThrough | De datum om het werk bij te werken tot voltooid. |
| setZeroOrHundredPercentCompleteOnly | Indien ingesteld op true, werkt alleen die taken bij als 100% voltooid waarvan de einddatum vóór de opgegeven voltooid‑tot datum ligt. Anders wordt een voltooiingspercentage berekend op basis van de geplande start‑ en voltooid‑tot datums. |
| taskCollection | Lijst< Task > met taken waarvoor het werk moet worden bijgewerkt. |

