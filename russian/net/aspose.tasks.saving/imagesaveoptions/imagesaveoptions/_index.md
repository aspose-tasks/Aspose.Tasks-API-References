---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ImageSaveOptions. Инициализирует новый экземпляр класса ImageSaveOptions, который можно использовать для сохранения отрисованных изображений в форматах TIFF, PNG, BMP или JPEG"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Инициализирует новый экземпляр класса [`ImageSaveOptions`](../), который можно использовать для сохранения отрисованных изображений в форматах TIFF, PNG, BMP или JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Может быть TIFF, PNG, BMP или JPEG[`SaveFileFormat`](../../savefileformat/). |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Выбрасывается, если *saveFormat* не является допустимым форматом изображения. Допустимые значения: TIFF, PNG, BMP или JPEG. |

## Примеры

Показывает, как сохранить проект в поток в виде изображения.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // используя ImageSaveOptions, мы сохраняем проект в формате изображения
    project.Save(stream, options);
}
```

### См. также

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


