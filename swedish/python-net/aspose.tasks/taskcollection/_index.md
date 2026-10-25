---
title: "TaskCollection"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 1140
url: /sv/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Representerar en samling av [Task](/tasks/python-net/aspose.tasks/task/) objekt.

Typen TaskCollection visar följande medlemmar:
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| parent_project | Hämtar det överordnade projektet för TaskCollection-objektet. |
## Methods
| Namn | Beskrivning |
| :- | :- |
| add() | Lägg till den angivna uppgiften i en instans av klassen [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Om ParentProject.CalculationMode är None bör användaren anropa Project.Recalculate() efter att ha använt denna metod (Den kommer att omplanera alla projektuppgifter (start-/slutdatum, sätter tidiga/sena datum) och beräkna de beroende fälten såsom slack, arbete och kostnadsfält, id:n och outline-nivåer).<br/>            Om ParentProject.CalculationMode är Manual kommer metoden endast att beräkna uppgifts-id, outline-nivå och outline-nummer automatiskt.<br/>            Om ParentProject.CalculationMode är Automatic omplanerar metoden alla projektets uppgifter automatiskt<br/>            (start-/slutdatum, sätter tidiga/sena datum, beräknar slack, arbete och kostnadsfält, omberäknar  id:n och outline-nivåer). |
| add(task_name) | Lägger till en ny uppgift i samlingen av underordnade uppgifter. |
| add(task_name, before_task_id) |  |
| add(parameters) | Infogar en ny uppgift före en uppgift med det angivna id:t och på samma outline-nivå. |
| to_list() | Konverterar TaskCollection-objektet till en lista med [Task](/tasks/python-net/aspose.tasks/task/)-objekt. |
| get_by_uid(uid) | Returnerar en uppgift med det angivna Uid vars förfader är den överordnade uppgiften i denna samling. |
| get_by_id(id) | Returnerar en uppgift med det angivna Id vars förfader är den överordnade uppgiften i denna samling. |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

