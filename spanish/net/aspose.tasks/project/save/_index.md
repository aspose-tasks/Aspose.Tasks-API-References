---
title: "Project.Save"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Guarda el documento en un archivo usando las opciones de guardado especificadas"
type: docs
weight: 1200
url: /es/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

Guarda el documento en un archivo usando las opciones de guardado especificadas.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | Cadena | El nombre del archivo. |
| opciones | SimpleSaveOptions | Las opciones de guardado. |

## Ejemplos

Muestra cómo guardar el proyecto como un archivo MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### Ver también

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

Guarda los datos del proyecto en el archivo.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | Cadena | El nombre del archivo. |
| formato | SaveFileFormat | El formato de archivo de guardado. |

## Ejemplos

Muestra cómo crear un proyecto y guardarlo en formato MPP sin pasar un archivo de plantilla MPP.

```csharp
var project = new Project();

// El proyecto se guardará en MPP utilizando una plantilla MPP interna.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

Guarda los datos del proyecto en el archivo en formato mpp.

```csharp
public void Save(string filename)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | Cadena | El nombre del archivo. |

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

Guarda el proyecto en un flujo usando las opciones de guardado especificadas.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo. |
| opciones | SimpleSaveOptions | Las opciones de guardado. |

## Ejemplos

Muestra cómo guardar el proyecto en un flujo como un archivo MPP usando las opciones de guardado MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // mediante el uso de MPPSaveOptions lo guardamos en formato MPP
    project.Save(stream, options);
}
```

Muestra cómo guardar el proyecto en un flujo como una imagen y controlar las opciones de imagen.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // usando ImageSaveOptions guardamos el proyecto en formato de imagen
    project.Save(stream, options);
}
```

### Ver también

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

Guarda los datos del proyecto en el flujo.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo. |
| format | SaveFileFormat | el formato de archivo de guardado especificado.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## Ejemplos

Muestra cómo guardar el proyecto en un flujo como un archivo XML de MS Project.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // Escribe el flujo en formato XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### Ver también

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


