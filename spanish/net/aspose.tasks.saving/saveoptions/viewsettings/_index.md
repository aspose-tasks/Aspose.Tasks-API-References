---
title: SaveOptions.ViewSettings
second_title: Referencia de Aspose.Tasks para la API de .NET
description: SaveOptions propiedad. Obtiene o establece una vista View  para renderizar. Puede usar estas opciones para especificar explícitamente qué vista debe guardarse en formato PDF HTML o de imagen. Si se establece esta propiedadPresentationFormat La propiedad se ignora cuando se guarda el proyecto. La vista debe ser desde una de las siguientes pantallas Screen  Gantt Hoja de tareas Uso de tareas Hoja de recursos Uso de recursos
type: docs
weight: 240
url: /es/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Obtiene o establece una vista ([`View`](../view/) ) para renderizar. Puede usar estas opciones para especificar explícitamente qué vista debe guardarse en formato PDF, HTML o de imagen. Si se establece esta propiedad,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) La propiedad se ignora cuando se guarda el proyecto. La vista debe ser desde una de las siguientes pantallas (([`Screen`](../../../aspose.tasks/view/screen/) )): (Gantt, Hoja de tareas, Uso de tareas, Hoja de recursos, Uso de recursos)

```csharp
public View ViewSettings { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando se llama al método set y se proporciona una instancia de la clase View con un valor no admitido de la propiedad Screen. |

### Ver también

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* espacio de nombres [Aspose.Tasks.Saving](../../saveoptions/)
* asamblea [Aspose.Tasks](../../../)


