---
title: Metered.SetMeteredKey
second_title: Aspose.Tasks för .NET API-referens
description: Metered metod. Ställer in mätta offentliga och privata nycklar.
type: docs
weight: 30
url: /sv/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ställer in mätta offentliga och privata nycklar.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| publicKey | String | Den publika nyckeln. |
| privateKey | String | Den privata nyckeln. |

### Anmärkningar

Om du köper mätlicens bör detta API anropas vid start av applikationen, normalt räcker detta. Men om mätt inte laddar upp förbrukningsdata under 24 timmar kommer licensen att ställas in på utvärderingsstatus. För att undvika sådana fall bör du regelbundet kontrollera licensstatusen Om det är utvärderingsstatus, anropa detta API igen.

### Se även

* class [Metered](../)
* namnutrymme [Aspose.Tasks](../../metered/)
* hopsättning [Aspose.Tasks](../../../)


