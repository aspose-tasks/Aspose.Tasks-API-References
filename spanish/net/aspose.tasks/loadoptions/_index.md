---
title: "Clase LoadOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.LoadOptions. Permite especificar parámetros de carga adicionales al cargar un proyecto desde un archivo o flujo."
type: docs
weight: 990
url: /es/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Permite especificar parámetros de carga adicionales al cargar un proyecto desde un archivo o flujo.

```csharp
public class LoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LoadOptions](loadoptions/)() | Inicializa una nueva instancia de la clase `LoadOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Obtiene o establece un token que puede usarse para cancelar una operación de carga de proyecto. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Obtiene o establece la codificación que se usa para leer un proyecto desde formatos HTML, MPX, XER y Primavera XML. La codificación predeterminada es UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Obtiene o establece un método de devolución de llamada para manejar errores de análisis XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Obtiene o establece una contraseña de protección. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Obtiene o establece una instancia especificada de la clase [`PrimaveraReadOptions`](../primaverareadoptions/) que puede usarse para personalizar el comportamiento de carga de formatos Primavera (Primavera P6 XER o Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Obtiene o establece la devolución de llamada que se invocará durante las operaciones de carga de proyecto. Actualmente compatible con los formatos MPP y XER. |

## Ejemplos

Muestra cómo cargar el proyecto protegido con contraseña usando una instancia de &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


