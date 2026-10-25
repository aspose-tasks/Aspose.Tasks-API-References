---
title: "Project.CopyTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Project. Copia los datos principales y propiedades del proyecto a otro proyecto."
type: docs
weight: 1060
url: /es/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Copia los datos principales y las propiedades del proyecto a otro proyecto.

```csharp
public void CopyTo(Project another)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Project | Otro proyecto al que copiar los datos. |

## Ejemplos

Muestra cómo copiar los datos del proyecto a otro proyecto.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// omitir la copia de datos de vista al copiar datos comunes del proyecto.
project.CopyTo(mppProject);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Copia los datos principales y las propiedades del proyecto a otro proyecto.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Project | Otro proyecto al que copiar los datos. |
| opciones | CopyToOptions | Opciones de copia para controlar el proceso de copia. |

## Ejemplos

Muestra cómo copiar el proyecto con el uso de &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt; instancia.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// omitir la copia de datos de vista al copiar datos comunes del proyecto.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### Ver también

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


