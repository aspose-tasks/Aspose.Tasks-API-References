---
title: "Aspose::Tasks::Project::Recalculate Methode"
linktitle: "Neu berechnen"
articleTitle: "Neu berechnen"
second_title: "Aspose.Tasks für C++"
description: "Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spättermine, berechnet Puffer, Arbeits- und Kostenfelder."
type: docs
weight: 1130
url: /de/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spättermine, berechnet Puffer, Arbeits- und Kostenfelder.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spätdaten, berechnet Puffer, Arbeits- und Kostenfelder mit optionaler Validierung.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parameter | Beschreibung |
| --- | --- |
| validieren | Wenn true, wird die Validierung der Neuberechnung durchgeführt. Welche Daten validiert werden: Derzeit ist nur eine grundlegende Validierung von Aufgaben- und Aufgabenverknüpfungs-Datumsbereichen implementiert. Die Datumsbereiche von Aufgaben (z. B. ActualStart - ActualFinish, EarlyStart - EarlyFinish usw.) sowie die Daten von Aufgabenverknüpfungen werden anhand des Kriteriums geprüft, dass das Startdatum kleiner oder gleich dem Enddatum ist. Wenn eine der oben beschriebenen Bedingungen fehlschlägt, wird eine RecalculationValidationException ausgelöst. |

