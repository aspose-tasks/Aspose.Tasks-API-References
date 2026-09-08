---
title: "Project.GetDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Obtiene un objeto Duration con el número especificado de unidades y el formato de duración predeterminado que se define en la configuración de proyectos DurationFormat."
type: docs
weight: 1100
url: /es/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Obtiene el objeto [`Duration`](../../duration/) con el número especificado de unidades y el formato de duración predeterminado que se define en la configuración del proyecto [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | Double | número especificado de unidades. |

### Valor devuelto

Objeto Duration.

## Observaciones

Este método debe usarse con cuidado porque devuelve duraciones diferentes según la configuración Project.DurationFormat. Por ejemplo, GetWork(1.0) devolverá 1 hora cuando Project.DurationFormat sea TimeUnitType.Hour o 1 día si Project.DurationFormat es TimeUnitType.Day.

## Ejemplos

Muestra cómo crear una instancia &lt;see cref="Aspose.Tasks.Duration" /&gt; con el formato de duración predeterminado del proyecto mediante los métodos de fabricación del proyecto.

```csharp
var project = new Project();

// obtener una duración con el formato predeterminado del proyecto.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Ver también

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Obtiene el objeto [`Duration`](../../duration/) con el número especificado de unidades [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | Double | número especificado de unidades. |
| timeUnit | TimeUnitType | valor especificado de TimeUnitType. |

### Valor devuelto

Objeto Duration.

## Ejemplos

Muestra cómo crear una instancia &lt;see cref="Aspose.Tasks.Duration" /&gt; mediante los métodos de fabricación del proyecto.

```csharp
var project = new Project();

// obtener una duración con el formato predeterminado del proyecto.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Ver también

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Obtiene el objeto [`Duration`](../../duration/) con el valor especificado de TimeSpan y el valor especificado de [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| timeSpan | TimeSpan | valor especificado de TimeSpan. |
| timeUnit | TimeUnitType | valor especificado de TimeUnitType. |

### Valor devuelto

Objeto Duration.

### Ver también

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


