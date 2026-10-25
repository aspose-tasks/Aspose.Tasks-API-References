---
title: "Klasse Project"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Project‑klasse. Vertegenwoordigt een project"
type: docs
weight: 1440
url: /nl/net/aspose.tasks/project/
---
## Project class

Stelt een project voor.

```csharp
public class Project
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Project](project/#constructor)() | Initialiseert een nieuwe instantie van de `Project`‑klasse. |
| [Project](project/#constructor_1)(DbSettings) | Initialiseert een nieuwe instantie van de `Project`‑klasse om gegevens te lezen uit een database die wordt gespecificeerd door de instantie van de [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/)‑klasse. |
| [Project](project/#constructor_2)(Stream) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een stream. |
| [Project](project/#constructor_7)(StreamReader) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een StreamReader‑instantie. |
| [Project](project/#constructor_8)(string) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit de Stream met de opgegeven instantie van de [`LoadOptions`](../loadoptions/)‑klasse. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon(bestaand mpp‑ of mpt‑bestand). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit de Stream met de opgegeven instantie van de [`PrimaveraReadOptions`](../primaverareadoptions/)‑klasse. |
| [Project](project/#constructor_6)(Stream, string) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon(bestaand mpp‑ of mpt‑bestand). |
| [Project](project/#constructor_9)(string, LoadOptions) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon (bestaand MPP‑ of MPT‑bestand) met de opgegeven instantie van de [`LoadOptions`](../loadoptions/)‑klasse. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon (bestaand mpp‑ of mpt‑bestand). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Initialiseert een nieuwe instantie van de `Project`‑klasse vanuit een sjabloon (bestaand MPP‑ of MPT‑bestand) met de opgegeven instantie van de [`PrimaveraReadOptions`](../primaverareadoptions/)‑klasse. |
| [Project](project/#constructor_12)(string, string) | Initialiseert een nieuw exemplaar van de `Project`-klasse vanuit een met wachtwoord beveiligde sjabloon (bestaand mpp- of mpt‑bestand). |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of ActualsInSync is ingesteld of niet. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of AdminProject is ingesteld of niet. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of AreEditableActualCosts is ingesteld of niet. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Haalt op of stelt een waarde van Author in. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Haalt op of stelt in of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk van de toewijzing en de tarieven van de bron. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of Autolink is ingesteld of niet. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Haalt op of stelt een waarde van BaselineForEarnedValue in. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Haalt de ingebouwde eigenschapencollectie van het project op. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Haalt op of stelt de berekeningsmodus van een project in. Kan een van de waarden van de enumeratie [`CalculationMode`](./calculationmode/) zijn. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Haalt of stelt een waarde van Calendar in. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Haalt het [`CalendarCollection`](../calendarcollection/)‑object van deze Project‑instantie op. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Haalt op of stelt een waarde van Category in. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Haalt op of stelt een waarde van Comments in. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Haalt op of stelt een waarde van Company in. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Haalt op of stelt een waarde van CreationDate in. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Haalt een collectie op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen. Dit is een O(n)-operatie, waarbij n het aantal taken in het project is. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Taken worden door MS Project als kritisch beschouwd als de totale speling kleiner of gelijk is aan dit aantal dagen. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Haalt op of stelt een waarde van CurrencyCode in. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Haalt op of stelt een waarde van CurrencyDigits in. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Haalt op of stelt een waarde van CurrencySymbol in. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Haalt op of stelt een waarde van CurrencySymbolPosition in. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Haalt op of stelt een waarde van CurrentDate in. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Haalt op of stelt een waarde van CustomDateFormat in. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Haalt de aangepaste eigenschapencollectie van het project op. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Haalt een waarde op of stelt een waarde in van DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Haalt een waarde op of stelt een waarde in van DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Haalt een waarde op of stelt een waarde in van DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Haalt de standaardweergave van het project op of stelt deze in. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Haalt de instantie op van de [`WeekDayCollection`](../weekdaycollection/) klasse die een verzameling van project‑standaard weekwerkdagen en werktijden vertegenwoordigt. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Haalt een instantie op van de [`ProjectDisplayOptions`](../projectdisplayoptions/) klasse. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Haalt een waarde op of stelt een waarde in van DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Haalt een waarde op of stelt een waarde in van EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Haalt het ExtendedAttributeDefinitionCollection‑object op. De verzameling van definities van uitgebreide attributen (aangepaste velden) die aan een project zijn gekoppeld. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Haalt een waarde op of stelt een waarde in van ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Haalt een waarde op of stelt een waarde in van FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of FiscalYearStart is ingesteld of niet. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Haalt een waarde op of stelt een waarde in van FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Haalt de globalisatie‑ (taalspecifieke) instellingen van het project op of stelt deze in. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Haalt of stelt een waarde van Guid in. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of HonorConstraints is ingesteld of niet. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Haalt een waarde op of stelt een waarde in van HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Haalt een waarde op of stelt een waarde in van Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Haalt een waarde op of stelt een waarde in van LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Haalt een waarde op of stelt een waarde in van LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Haalt een waarde op of stelt een waarde in van LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Haalt een waarde op of stelt een waarde in van Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MicrosoftProjectServerURL is ingesteld of niet. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Haalt een waarde op of stelt een waarde in van MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Haalt een waarde op of stelt een waarde in van MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MoveCompletedEndsBack is ingesteld of niet. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MoveCompletedEndsForward is ingesteld of niet. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MoveRemainingStartsBack is ingesteld of niet. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MoveRemainingStartsForward is ingesteld of niet. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of MultipleCriticalPaths is ingesteld of niet. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Haalt een waarde op of stelt deze in van Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of NewTasksAreManual is ingesteld of niet. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of NewTasksEffortDriven is ingesteld of niet. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of NewTasksEstimated is ingesteld of niet. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Haalt een waarde op of stelt een waarde in van NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Haalt een collectie op die de instanties van de [`OleObject`](../oleobject/) klasse bevat die gekoppeld of ingesloten zijn in dit projectbestand. Alleen beschikbaar voor mpp-bestandsformaat. Deze collectie is alleen-lezen, behalve voor de 'Clear'-bewerking. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Haalt OutlineCodeDefinitionCollection-object op. De collectie van outline code-definities die aan een project zijn gekoppeld. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Haalt een object op dat Primavera-specifieke eigenschappen bevat voor een project dat uit een Primavera-bestand is gelezen. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of ProjectExternallyEdited is ingesteld of niet. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of RemoveFileProperties is ingesteld of niet. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Haalt ResourceAssignmentCollection-object op. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Haalt alle resource-gebaseerde filterdefinities op. ResourceFilters is een collectie van [`Filter`](../filter/) objecten. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Haalt alle resource-gebaseerde groepsdefinities op. ResourceGroups is een collectie van [`Group`](../group/) objecten. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Haalt ResourceCollection-object op. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Haalt een waarde van Revisie op of stelt deze in. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Haalt de root van de taakboom op. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Haalt een waarde van SaveVersion op of stelt deze in. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Haalt een waarde op die aangeeft of ScheduleFromStart is ingesteld of niet, of stelt deze in. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Haalt een waarde op die aangeeft of ShowProjectSummaryTask is ingesteld of niet, of stelt deze in. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Haalt een waarde op die aangeeft of SplitsInProgressTasks is ingesteld of niet, of stelt deze in. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Haalt een waarde op die aangeeft of SpreadActualCost is ingesteld of niet, of stelt deze in. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Haalt een waarde op die aangeeft of SpreadPercentComplete is ingesteld of niet, of stelt deze in. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Haalt een waarde van StartDate op of stelt deze in. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Haalt een waarde van StatusDate op of stelt deze in. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Haalt een waarde van Subject op of stelt deze in. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Haalt een lijst met [`Table`](../table/) objecten op. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Haalt alle taakgebaseerde filterdefinities op. TaskFilters is een collectie van [`Filter`](../filter/) objecten. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Haalt alle taakgebaseerde groepsdefinities op. TaskGroups is een collectie van [`Group`](../group/) objecten. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Haalt [`TaskLinkCollection`](../tasklinkcollection/) object op. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Haalt een waarde op die aangeeft of TaskUpdatesResource is ingesteld of niet, of stelt deze in. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Haalt een waarde van Template op of stelt deze in. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Haalt een waarde van TimescaleFinish op of stelt deze in. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Haalt een waarde van TimescaleStart op of stelt deze in. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Haalt een waarde van Title op of stelt deze in. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Haalt een waarde op of stelt een waarde in voor Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Haalt een waarde op die aangeeft of UpdateManuallyScheduledTasksWhenEditingLinks is ingesteld of niet, of stelt deze in. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Haalt een instantie van de [`VbaProject`](./vbaproject/) klasse op. |
| [Views](../../aspose.tasks/project/views/) { get; } | Haalt een lijst met [`View`](../view/) objecten op. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Haalt de WBS-code-definitie voor het project op of stelt deze in. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Haalt een waarde van WeekStartDay op of stelt deze in. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Haalt een waarde op of stelt een waarde in van WorkFormat. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Doorloopt recursief alle taken van het project, inclusief de hoofdtaak. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Retourneert de baseline-opslagtijd. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Haalt een [`Duration`](../duration/) object op met het opgegeven aantal eenheden en het standaardduurformaat dat is gedefinieerd in de projectinstellingen [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Haalt een [`Duration`](../duration/) object op met het opgegeven aantal [`TimeUnitType`](../timeunittype/) eenheden. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Haalt een [`Duration`](../duration/) object op met de opgegeven TimeSpan-waarde en de opgegeven [`TimeUnitType`](../timeunittype/) waarde. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard [`Timescale`](../../aspose.tasks.visualization/timescale/)(Dagen). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard [`Timescale`](../../aspose.tasks.visualization/timescale/)(Dagen) en de opgegeven [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`SaveOptions`](../../aspose.tasks.saving/saveoptions/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../aspose.tasks.visualization/timescale/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../aspose.tasks.visualization/timescale/) en [`PageSize`](../../aspose.tasks.visualization/pagesize/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../aspose.tasks.visualization/timescale/) en [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) en datumbereik. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Retourneert een verzameling taaklinks die voorlopers zijn van de opgegeven taak. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Haalt een [`Duration`](../duration/) object op met de opgegeven Double-waarde en het standaard werkformaat. |
| [Print](../../aspose.tasks/project/print/#print)() | Print het project naar de standaardprinter met de standaardprinterinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Print het project naar de standaardprinter met de standaardprinterinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Print het project naar de opgegeven printer met de standaardprinterinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Print het project volgens de opgegeven printerinstellingen en aangepaste opslagopties met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Print het project volgens de opgegeven printerinstellingen met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Print het project volgens de opgegeven printerinstellingen, aangepaste opslagopties en de opgegeven documentnaam met behulp van de standaard (geen gebruikersinterface) printcontroller. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Plant alle taak‑ID's, outline‑niveaus, start-/einddatums van het project opnieuw in, stelt vroege/late datums in, berekent speling, werk‑ en kostvelden. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Plant alle taak‑ID's, outline‑niveaus, start-/einddatums van het project opnieuw in, stelt vroege/late datums in, berekent speling, werk‑ en kostvelden met optionele validatie. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Herberekent Id, Start en Finish van resources. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Verwijdert ongeldige resource-toewijzingen uit de lijst met projectresource-toewijzingen. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Her nummer WBS-code van alle taken. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Her nummer WBS-code van voltooide taken. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Plant onvoltooide projectwerk opnieuw in om te starten na een opgegeven datum. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Plant onvoltooide werkzaamheden voor een opgegeven lijst met taken opnieuw in om te starten na een opgegeven datum. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Slaat de projectgegevens op in het bestand in mpp-indeling. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Slaat de projectgegevens op in de stream. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Slaat het project op in een stream met behulp van de opgegeven opslagopties. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Slaat de projectgegevens op in het bestand. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Slaat het document op in een bestand met behulp van de opgegeven opslagopties. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Slaat het project op als sjabloon in een opgegeven stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Slaat het project op als sjabloon op het opgegeven bestandspad. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Slaat het project op als sjabloon in een opgegeven stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Slaat het project op als sjabloon. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Slaat het projectoverzichtsrapport op in de stream. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Slaat het projectoverzichtsrapport op in een PDF-bestand. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Slaat het projectrapport van het opgegeven type op in de opgegeven stream. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Slaat het projectrapport van het opgegeven type in PDF-indeling op op het opgegeven bestandspad. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Verzamelt recursief alle onderliggende taken van de hoofdtaak. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Slaat baseline-velden op naar de opgegeven baseline voor het gehele project. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Slaat baseline-velden op naar de opgegeven baseline voor de geselecteerde taken. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Stelt de baseline-opslagtijd in. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Markeert al het werk als voltooid tot een opgegeven datum voor het gehele project. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Markeert al het werk als voltooid tot een opgegeven datum voor de opgegeven lijst met taken. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Haalt projectbestandsinformatie op uit de stream. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Leest projectbestandsinformatie uit het bestand. |

## Opmerkingen

De **Project** is een centrale klasse in de Aspose.Tasks-bibliotheek.

U kunt **Project** gebruiken om een van de ondersteunde projectmanagementformaten te lezen: MPP, MPT, MPX, XML.

Om een bestaand document in een van de ondersteunde formaten te laden, geeft u een bestandsnaam of een stream door aan een van de **Project**-constructors. Om een leeg project te maken, roept u de parameterloze constructor aan.

Gebruik een van de Save-methode-overloads om het project op te slaan in een van de [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) formaten: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Afbeeldingen: JPEG, PNG, BMP, TIFF, SVG; Tekst: TXT; Overige: HTML.

De **Project** slaat projectbrede informatie op, zoals [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), en [`ExtendedAttributes`](./extendedattributes/). De meeste van deze objecten zijn toegankelijk via de overeenkomstige eigenschappen van de **Project**-klasse.

De **Project** is een root‑entity die toegangspunten bevat om andere project‑entity's te manipuleren, zoals [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) en [`Calendar`](../calendar/).

De **Project**‑entity's kunnen worden benaderd via getypeerde collecties, bijvoorbeeld [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), enzovoort.

## Voorbeelden

Toont hoe te werken met een &lt;see cref=\"Aspose.Tasks.Project\"/&gt; instantie.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// nieuwe taken toevoegen en gewenste eigenschappen instellen
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// nieuwe resources toevoegen
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// nieuwe resource‑toewijzingen toevoegen
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// project opslaan in een van de beschikbare formaten
// hier slaan we het op in Microsoft Project XML‑bestandformaat.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


