---
title: Project.Recalculate
second_title: Aspose.Tasks für .NET-API-Referenz
description: Project methode. Plant alle ProjektaufgabenIDs Gliederungsebenen Start/Endtermine neu legt frühe/späte Termine fest berechnet Lücken Arbeits und Kostenfelder.
type: docs
weight: 1120
url: /de/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Endtermine neu, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder.

```csharp
public void Recalculate()
```

### Siehe auch

* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Endtermine neu, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder mit optionaler Validierung.

```csharp
public void Recalculate(bool validate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| validate | Boolean | Wenn wahr, wird die Validierung der Neuberechnung durchgeführt. Welche Daten werden validiert: Im Moment ist nur die grundlegende Validierung der Datumsbereiche von Aufgaben und Aufgabenverknüpfungen implementiert. Die Datumsbereiche von Aufgaben (z. B. ActualStart - ActualFinish, EarlyStart - EarlyFinish usw. ) sowie Aufgabenverknüpfungsdaten werden anhand der Datumskriterien überprüft, dass das Startdatum kleiner oder gleich dem Enddatum ist. Wenn eine der oben beschriebenen Bedingungen fehlschlägt, dann[`RecalculationValidationException`](../../recalculationvalidationexception/)wird geworfen. |

### Siehe auch

* class [Project](../)
* namensraum [Aspose.Tasks](../../project/)
* Montage [Aspose.Tasks](../../../)


