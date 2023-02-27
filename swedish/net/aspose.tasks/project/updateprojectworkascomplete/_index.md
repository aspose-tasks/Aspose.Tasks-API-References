---
title: Project.UpdateProjectWorkAsComplete
second_title: Aspose.Tasks för .NET API-referens
description: Project metod. Uppdaterar allt arbete som komplett till ett angivet datum för hela projektet.
type: docs
weight: 1250
url: /sv/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Uppdaterar allt arbete som komplett till ett angivet datum för hela projektet.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| completeThrough | DateTime | Datumet för att uppdatera arbetet som slutfört till och med. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Om den är inställd på sanna uppdaterar endast de uppgifter som 100 % slutförda vars slutdatum ligger före det angivna slutdatumet. I annat fall beräknas ett procentuellt värde baserat på schemalagda start- och slutdatum. |

### Se även

* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Uppdaterar allt arbete som komplett till ett angivet datum för den angivna listan med uppgifter.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| completeThrough | DateTime | Datumet för att uppdatera arbetet som slutfört till och med. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Om den är inställd på sanna uppdaterar endast de uppgifter som 100 % slutförda vars slutdatum ligger före det angivna slutdatumet. I annat fall beräknas ett procentuellt värde baserat på schemalagda start- och slutdatum. |
| taskCollection | List`1 | Lista&lt;Uppgift&gt; över uppgifter att uppdatera arbete för. |

### Se även

* class [Task](../../task/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)


