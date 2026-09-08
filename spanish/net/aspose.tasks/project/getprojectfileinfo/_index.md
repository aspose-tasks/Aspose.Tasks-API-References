---
title: "Project.GetProjectFileInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Lee la información del archivo de proyecto desde el archivo"
type: docs
weight: 1280
url: /es/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Lee la información del archivo del proyecto del archivo.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | Cadena | El nombre de archivo del proyecto. |

### Valor devuelto

La información del archivo de proyecto [`ProjectFileInfo`](../../projectfileinfo/).

## Ejemplos

Muestra cómo leer la información del archivo de proyecto desde un archivo XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Obtiene la información del archivo del proyecto del flujo.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo de datos. |

### Valor devuelto

La información del archivo de proyecto [`ProjectFileInfo`](../../projectfileinfo/).

## Ejemplos

Muestra cómo leer la información del archivo de proyecto de un archivo XML leído desde un flujo.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Ver también

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


