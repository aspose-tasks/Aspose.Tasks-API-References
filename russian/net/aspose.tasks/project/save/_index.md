---
title: "Project.Save"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Сохраняет документ в файл, используя указанные параметры сохранения"
type: docs
weight: 1200
url: /ru/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Сохраняет документ в файл, используя указанные параметры сохранения.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | Строка | Имя файла. |
| опции | SimpleSaveOptions | Параметры сохранения. |

## Примеры

Показывает, как сохранить проект в файл MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### См. также

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Сохраняет данные проекта в файл.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | Строка | Имя файла. |
| формат | SaveFileFormat | Формат файла сохранения. |

## Примеры

Показывает, как создать проект и сохранить его в формате MPP без использования шаблона MPP.

```csharp
var project = new Project();

// Проект будет сохранён в формате MPP с использованием внутреннего шаблона MPP.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Сохраняет данные проекта в файл в формате mpp.

```csharp
public void Save(string filename)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | Строка | Имя файла. |

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Сохраняет проект в поток, используя указанные параметры сохранения.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток. |
| опции | SimpleSaveOptions | Параметры сохранения. |

## Примеры

Показывает, как сохранить проект в поток в виде файла MPP, используя параметры сохранения MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // Используя MPPSaveOptions, мы сохраняем его в формате MPP.
    project.Save(stream, options);
}
```

Показывает, как сохранить проект в поток в виде изображения и управлять параметрами изображения.

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

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Сохраняет данные проекта в поток.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток. |
| format | SaveFileFormat | указанный формат файла сохранения.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Примеры

Показывает, как сохранить проект в поток в виде XML‑файла MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Записать поток в формат XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### См. также

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


