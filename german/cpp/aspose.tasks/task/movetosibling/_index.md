---
title: "Aspose::Tasks::Task::MoveToSibling Methode"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks für C++"
description: "Verschiebt die aktuelle Aufgabe auf derselben Gliederungsebene vor die angegebene Aufgabe."
type: docs
weight: 1370
url: /de/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Verschiebt die aktuelle Aufgabe auf derselben Outline‑Ebene vor die angegebene Aufgabe. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach Verwendung dieser Methode Project.Recalculate() aufrufen (dies wird alle Projektaufgaben neu planen (Start‑/Enddaten, setzt Früh‑/Spättermine) und die abhängigen Felder wie Puffer, Arbeits‑ und Kostenfelder sowie Outline‑Ebenen berechnen). Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur Aufgaben‑ID, Outline‑Ebene und Outline‑Nummern automatisch. Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Projektaufgaben automatisch neu (Start‑/Enddaten, setzt Früh‑/Spättermine, berechnet Puffer, Arbeits‑ und Kostenfelder, recalculates IDs und Outline‑Ebenen).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parameter | Beschreibung |
| --- | --- |
| beforeTask | Aufgabe, vor der die aktuelle Aufgabe eingefügt wird. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Verschiebt die aktuelle Aufgabe auf derselben Gliederungsebene vor eine Aufgabe mit der angegebenen Id. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer nach der Verwendung dieser Methode Project.Recalculate() aufrufen (Sie wird alle Projektaufgaben neu planen (Start-/Enddaten, legt Früh-/Spättermine fest) und die abhängigen Felder wie Puffer, Arbeits- und Kostendaten sowie Gliederungsebenen berechnen). Wenn ParentProject.CalculationMode Manual ist, berechnet die Methode nur die Aufgaben‑Id, die Gliederungsebene und die Gliederungsnummern automatisch. Wenn ParentProject.CalculationMode Automatic ist, plant die Methode alle Aufgaben des Projekts automatisch neu (Start-/Enddaten, legt Früh-/Spättermine fest, berechnet Puffer, Arbeits- und Kostendaten, berechnet Ids und Gliederungsebenen neu).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parameter | Beschreibung |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) einer Aufgabe, vor der die aktuelle Aufgabe eingefügt wird. |

