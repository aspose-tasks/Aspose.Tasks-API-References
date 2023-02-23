---
title: SaveOptions.ViewSettings
second_title: Справочник по Aspose.Tasks для .NET API
description: SaveOptions свойство. Получает или задает представление View  для рендеринга. Вы можете использовать эти параметры чтобы явно указать какое представление должно быть сохранено в форматах PDF HTML или Image. Если это свойство установленоPresentationFormat свойство игнорируется при сохранении проекта. Вид должен быть на одном из следующих экранов Screen  Ганта TaskSheet TaskUsage ResourceSheet ResourceUsage
type: docs
weight: 240
url: /ru/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Получает или задает представление ([`View`](../view/) ) для рендеринга. Вы можете использовать эти параметры, чтобы явно указать, какое представление должно быть сохранено в форматах PDF, HTML или Image. Если это свойство установлено,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) свойство игнорируется при сохранении проекта. Вид должен быть на одном из следующих экранов (([`Screen`](../../../aspose.tasks/view/screen/) )): (Ганта, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Когда вызывается метод set и предоставляется экземпляр класса View с неподдерживаемым значением свойства Screen. |

### Смотрите также

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* пространство имен [Aspose.Tasks.Saving](../../saveoptions/)
* сборка [Aspose.Tasks](../../../)


