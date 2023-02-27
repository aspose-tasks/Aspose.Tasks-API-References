---
title: TimephasedDataCollection.CopyTo
second_title: Aspose.Tasks für .NET-API-Referenz
description: TimephasedDataCollection methode. Kopiert die Elemente derTimephasedDataCollection zu einemArray  ab einem bestimmtenArray index.
type: docs
weight: 90
url: /de/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Kopiert die Elemente der[`TimephasedDataCollection`](../) zu einemArray , ab einem bestimmtenArray index.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| array | TimephasedData[] | Das EindimensionaleArray das ist das Ziel der kopierten Elemente[`TimephasedDataCollection`](../) . DieArray muss über eine nullbasierte Indizierung verfügen. |
| arrayIndex | Int32 | Der nullbasierte Index in*array* an dem der Kopiervorgang beginnt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *array* ist Null. |
| ArgumentOutOfRangeException | *arrayIndex* ist kleiner als 0. |
| ArgumentException | Die Anzahl der Elemente in der Quelle[`TimephasedDataCollection`](../) ist größer als der verfügbare Platz ab*arrayIndex* bis zum Ende des Ziels*array* . |

### Siehe auch

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* namensraum [Aspose.Tasks](../../timephaseddatacollection/)
* Montage [Aspose.Tasks](../../../)


