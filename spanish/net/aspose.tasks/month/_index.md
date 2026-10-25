---
title: "Enumeración Month"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Month. Especifica el mes"
type: docs
weight: 1040
url: /es/net/aspose.tasks/month/
---
## Month enumeration

Especifica el mes.

```csharp
public enum Month
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que el valor no estaba definido en el archivo de proyecto original. |
| January | `0` | Indica el mes de enero. |
| February | `1` | Indica el mes de febrero. |
| March | `2` | Indica el mes de marzo. |
| April | `3` | Indica el mes de abril. |
| May | `4` | Indica el mes de mayo. |
| June | `5` | Indica el mes de junio. |
| July | `6` | Indica el mes de julio. |
| August | `7` | Indica el mes de agosto. |
| September | `8` | Indica el mes de septiembre. |
| October | `9` | Indica el mes de octubre. |
| November | `10` | Indica el mes de noviembre. |
| December | `11` | Indica el mes de diciembre. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo trabajar con repeticiones de día del año al crear nuevas tareas recurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


