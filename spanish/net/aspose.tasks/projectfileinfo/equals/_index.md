---
title: "ProjectFileInfo.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ProjectFileInfo método. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 50
url: /es/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | ProjectFileInfo | El objeto especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si el ProjectFileInfo especificado y esta instancia tienen el mismo formato de archivo e información de aplicación.

## Ejemplos

Muestra cómo leer la información del archivo del proyecto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto especificado para comparar con esta instancia. |

### Valor devuelto

Devuelve true si el ProjectFileInfo especificado y esta instancia tienen el mismo formato de archivo e información de aplicación.

## Ejemplos

Muestra cómo leer la información del archivo del proyecto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


