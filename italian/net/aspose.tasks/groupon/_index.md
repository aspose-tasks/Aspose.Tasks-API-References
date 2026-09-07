---
title: "Enum GroupOn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.GroupOn. Specifica il tipo di raggruppamento"
type: docs
weight: 810
url: /it/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Specifica il tipo di raggruppamento.

```csharp
public enum GroupOn
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DateDay | `13` | Raggruppa per data per giorno. |
| DateEachValue | `10` | Raggruppa per data per ogni valore. |
| DateHour | `12` | Raggruppa per data per ora. |
| DateMinute | `11` | Raggruppa per data per minuto. |
| DateMonth | `16` | Raggruppa per data per mese. |
| DateQtr | `17` | Raggruppa per data per trimestre. |
| DateThirdOfMonth | `15` | Raggruppa per data per ogni terzo di un mese. |
| DateWeek | `14` | Raggruppa per data per settimana. |
| DateYear | `18` | Raggruppa per data per anno. |
| DurationDays | `23` | Raggruppa per durata per giorni. |
| DurationEachValue | `20` | Raggruppa per durata per ogni valore. |
| DurationHours | `22` | Raggruppa per durata per ore. |
| DurationMinutes | `21` | Raggruppa per durata per minuti. |
| DurationMonths | `25` | Raggruppa per durata per mesi. |
| DurationWeeks | `24` | Raggruppa per durata per settimane. |
| EachValue | `0` | Raggruppa per ogni valore. |
| Interval | `1` | Raggruppa per l'intervallo. |
| OutlineEachValue | `30` | Raggruppa per ogni valore di contorno. |
| OutlineLevel | `31` | Raggruppa per il livello di contorno. |
| Pct110 | `45` | Raggruppa per incrementi di completamento del 10%. |
| Pct125 | `44` | Raggruppa per incrementi di completamento del 25%. |
| Pct150 | `43` | Raggruppa per incrementi di completamento del 50%. |
| Pct199 | `42` | Raggruppa per completamento del 99%. |
| PctEachValue | `40` | Raggruppa per percentuale di ogni valore. |
| PctInterval | `41` | Raggruppa per la percentuale dell'intervallo. |
| TextEachValue | `50` | Raggruppa per ogni valore di testo. |
| TextPrefix | `51` | Raggruppa per il prefisso di testo. |

## Esempi

Mostra come leggere le proprietà di un criterio di gruppo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// leggi il modello di sfondo del criterio
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


