---
title: "Resource.GetTimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Resource. Devuelve una instancia de la clase TimephasedDataCollection para este objeto con los valores de TimephasedData dentro de las fechas de inicio y fin dadas del TimephasedDataType especificado"
type: docs
weight: 850
url: /es/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Devuelve una instancia de la clase [`TimephasedDataCollection`](../../timephaseddatacollection/) para este objeto con los valores de [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas del [`TimephasedDataType`](../../timephaseddatatype/) especificado.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio para los datos de tiempo faseado. |
| fin | DateTime | La fecha de fin para los datos de tiempo faseado. |
| timephasedType | TimephasedDataType | El tipo de datos de tiempo faseado ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Valor devuelto

Lista de [`TimephasedData`](../timephaseddata/).

## Ejemplos

Muestra cómo leer datos de tiempo faseado de recursos de trabajo/costo.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Obtenga el Resource por su ID
var resource = project.Resources.GetByUid(1);

// Imprime los datos de tiempo faseado de ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Imprime los datos de tiempo faseado de ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Devuelve [`TimephasedDataCollection`](../../timephaseddatacollection/) para este objeto con los valores de [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio para los datos de tiempo faseado. |
| fin | DateTime | La fecha de fin para los datos de tiempo faseado. |

### Valor devuelto

Lista de [`TimephasedData`](../../timephaseddata/).

## Ejemplos

Muestra cómo leer datos de tiempo faseado de recursos de trabajo/costo.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Obtenga el Resource por su ID
var resource = project.Resources.GetByUid(1);

// Imprime los datos de tiempo faseado de ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Imprime los datos de tiempo faseado de ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


