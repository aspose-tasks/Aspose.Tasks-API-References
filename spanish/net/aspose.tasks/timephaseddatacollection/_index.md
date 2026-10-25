---
title: "Clase TimephasedDataCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TimephasedDataCollection. Representa una colección de objetos TimephasedData"
type: docs
weight: 2600
url: /es/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

Representa una colección de objetos [`TimephasedData`](../timephaseddata/).

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `TimephasedDataCollection`. |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | Obtiene un valor que indica si la ICollection es de solo lectura. |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. El accesor de establecimiento no es compatible. propiedad para establecer datos por fases de tiempo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | Añade una instancia de [`TimephasedData`](../timephaseddata/) a este objeto de colección. |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | Añade una colección de instancias de [`TimephasedData`](../timephaseddata/) a este objeto de colección. |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | Elimina todos los elementos de `TimephasedDataCollection`. |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | Determina si `TimephasedDataCollection` contiene un valor específico. |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | Copia los elementos de `TimephasedDataCollection` a una matriz, comenzando en un índice de matriz particular. |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | Elimina una instancia de [`TimephasedData`](../timephaseddata/) de este objeto de colección. |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | Selecciona todas las fases de tiempo entre *startTime* y *finishTime*. Tiene una complejidad O(log n) en el caso promedio. |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | Convierte el objeto `TimephasedDataCollection` en una lista de objetos [`TimephasedData`](../timephaseddata/). |

## Ejemplos

Muestra cómo trabajar con colecciones de datos por fases de tiempo.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var resource2 = project.Resources.Add("Resource 2");
resource2.Set(Rsc.Type, ResourceType.Work);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment2 = project.ResourceAssignments.Add(task2, resource2);
assignment2.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment2.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment2.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

// establecer contorno de trabajo contorneado
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// borrar tds generados
assignment.TimephasedData.Clear();

var td = new TimephasedData
             {
                 Start = new DateTime(2019, 11, 11, 8, 0, 0),
                 Finish = new DateTime(2019, 11, 11, 9, 0, 0),
                 Uid = assignment.Get(Asn.Uid),
                 Unit = TimeUnitType.Hour,
                 Value = "PT1H0M0S",
                 TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
             };
assignment.TimephasedData.Add(td);

var list = new List<TimephasedData>();
var td2 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 12, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 12, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
var td3 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };

list.Add(td2);
list.Add(td3);
assignment.TimephasedData.AddRange(list);

// se puede filtrar la colección por tipo y rango de fechas
Console.WriteLine("Print filtered tds:");
IList<TimephasedData> filteredTds = assignment.TimephasedData.SelectBetweenStartAndFinish(
    TimephasedDataType.AssignmentRemainingWork,
    new DateTime(2019, 11, 11, 0, 0, 0),
    new DateTime(2019, 11, 13));
foreach (var data in filteredTds)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("Timephased Data Type: " + data.TimephasedDataType);
    Console.WriteLine();
}

Console.WriteLine("--------------------------");
Console.WriteLine();

// ...
// agrega un td incorrecto y luego elimínalo
var td4 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT0H0M1S", // wrong value
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
assignment.TimephasedData.Add(td4);

// ...

// elimina el elemento td incorrecto
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// itera sobre los elementos con fase temporal
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// copia los tds a otra asignación
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// la colección puede convertirse en una lista simple
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// eliminemos los tds uno por uno
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### Ver también

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


