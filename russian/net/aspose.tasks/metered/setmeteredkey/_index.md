---
title: SetMeteredKey
second_title: Справочник по Aspose.Tasks для .NET API
description: Устанавливает лимитированные открытый и закрытый ключи.
type: docs
weight: 30
url: /ru/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Устанавливает лимитированные открытый и закрытый ключи.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | String | Открытый ключ. |
| privateKey | String | Закрытый ключ. |

### Примечания

Если вы покупаете лимитную лицензию, этот API должен вызываться при запуске приложения, обычно этого достаточно . Однако, если счетчик не загружает данные о потреблении в течение 24 часов, лицензия будет переведена в ознакомительный статус. Чтобы избежать такого случая, вы должны регулярно проверять статус лицензии. Если это статус оценки, снова вызовите этот API.

### Смотрите также

* class [Metered](../../metered)
* пространство имен [Aspose.Tasks](../../metered)
* сборка [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
