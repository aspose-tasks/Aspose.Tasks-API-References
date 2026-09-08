---
title: "Task.GetTimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Devuelve un objeto TimephasedDataCollection con valores TimephasedData dentro de las fechas de inicio y fin dadas del tipo de datos temporales especificado."
type: docs
weight: 1360
url: /es/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Devuelve un objeto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valores [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas del tipo de datos temporales especificado.

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

Un objeto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valores [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas del tipo de datos temporales especificado.

## Ejemplos

Muestra cómo obtener datos temporales (con tipo específico) de la tarea.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Devuelve un objeto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valores [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio para los datos de tiempo faseado. |
| fin | DateTime | La fecha de fin para los datos de tiempo faseado. |

### Valor devuelto

Lista de [`TimephasedData`](../../timephaseddata/) para completar.

## Ejemplos

Muestra cómo obtener datos por fase de tiempo (con tipo TaskWork) de la tarea.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


