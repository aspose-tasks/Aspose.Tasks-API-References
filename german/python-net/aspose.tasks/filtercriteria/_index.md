---
title: "FilterCriteria"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 350
url: /de/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Definiert die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden.

Der Typ FilterCriteria stellt die folgenden Mitglieder bereit:
## Konstruktoren
| Name | Beschreibung |
| :- | :- |
| FilterCriteria() | Initialisiert eine neue Instanz der Klasse FilterCriteria |
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| Operation | Liest oder setzt das Kriterium, das mit FieldName, Test und Value festgelegt wurde und sich auf andere Kriterien im Filter bezieht. |
| field | Liest oder setzt ein [field](/tasks/python-net/aspose.tasks/filtercriteria/) zum Ändern. |
| test | Liest oder setzt den Vergleichstyp, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Liest die Objektwerte, die mit dem Wert des mit FieldName angegebenen Feldes verglichen werden. |
| criteria_rows | Liest die Liste der untergeordneten [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) Zeilen.<br/>            Wenn der Filter mehr als eine Kriterienzeile enthält, bewirkt ein And-Operator, dass die Kriterien beider Zeilen erfüllt sein müssen, damit die Aufgabe oder Ressource als Ergebnis dieses Filters angezeigt wird.<br/>            Der Or-Operator bewirkt, dass die Kriterien einer der beiden Zeilen erfüllt sein müssen. |
## Methoden
| Name | Beschreibung |
| :- | :- |
| is_field_value() | Liest, ob der rechte Wert von FilterCriteria eine Feldreferenz und kein konstanter Wert ist. |
| set_value_field(value) | Setzt das Feld, dessen Wert mit dem Wert des durch FieldName angegebenen Feldes verglichen wird. |

### Siehe auch

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

