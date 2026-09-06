---
title: "Classe Project"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Project. Représente un projet"
type: docs
weight: 1440
url: /fr/net/aspose.tasks/project/
---
## Project class

Représente un projet.

```csharp
public class Project
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Project](project/#constructor)() | Initialise une nouvelle instance de la classe `Project`. |
| [Project](project/#constructor_1)(DbSettings) | Initialise une nouvelle instance de la classe `Project` pour lire des données depuis une base de données spécifiée par l'instance de la classe [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/). |
| [Project](project/#constructor_2)(Stream) | Initialise une nouvelle instance de la classe `Project` à partir d'un flux. |
| [Project](project/#constructor_7)(StreamReader) | Initialise une nouvelle instance de la classe `Project` à partir d'une instance de StreamReader. |
| [Project](project/#constructor_8)(string) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Initialise une nouvelle instance de la classe `Project` à partir du flux avec l'instance spécifiée de la classe [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Initialise une nouvelle instance de la classe `Project` à partir du flux avec l'instance spécifiée de la classe [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_6)(Stream, string) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project/#constructor_9)(string, LoadOptions) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la classe [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée de la classe [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_12)(string, string) | Initialise une nouvelle instance de la classe `Project` à partir d'un modèle protégé par mot de passe (fichier mpp ou mpt existant). |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Obtient ou définit une valeur indiquant si ActualsInSync est défini ou non. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Obtient ou définit une valeur indiquant si AdminProject est défini ou non. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Obtient ou définit une valeur indiquant si AreEditableActualCosts est défini ou non. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Obtient ou définit une valeur de Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Obtient ou définit une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Obtient ou définit si le coût d'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les tarifs des ressources. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Obtient ou définit une valeur indiquant si Autolink est défini ou non. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Obtient ou définit une valeur de BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Obtient la collection des propriétés intégrées du projet. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Obtient ou définit le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération [`CalculationMode`](./calculationmode/). |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Obtient ou définit une valeur de Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Obtient l'objet [`CalendarCollection`](../calendarcollection/) de cette instance de Project. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Obtient ou définit une valeur de Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Obtient ou définit une valeur de Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Obtient ou définit une valeur de Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Obtient ou définit une valeur de CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Obtient une collection qui contient une liste de tâches Critical qui composent le chemin critique de ce projet. Il s'agit d'une opération O(n), où n est le nombre de tâches du projet. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Les tâches sont considérées comme critiques par MS Project si le flottement total est inférieur ou égal à ce nombre de jours. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Obtient ou définit une valeur de CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Obtient ou définit une valeur de CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Obtient ou définit une valeur de CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Obtient ou définit une valeur de CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Obtient ou définit une valeur de CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Obtient ou définit une valeur de CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Obtient la collection des propriétés personnalisées du projet. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Obtient ou définit une valeur de DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Obtient ou définit une valeur de DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Obtient ou définit une valeur de DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Obtient ou définit une valeur de DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Obtient ou définit une valeur de DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Obtient ou définit une valeur de DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Obtient ou définit une valeur de DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Obtient ou définit une valeur de DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Obtient ou définit une valeur de DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Obtient ou définit la vue par défaut du projet. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Obtient l'instance de la classe [`WeekDayCollection`](../weekdaycollection/) qui représente une collection des jours de travail hebdomadaires par défaut du projet et des heures de travail. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Obtient une instance de la classe [`ProjectDisplayOptions`](../projectdisplayoptions/). |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Obtient ou définit une valeur de DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Obtient ou définit une valeur de EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Obtient l'objet ExtendedAttributeDefinitionCollection. La collection des définitions d'attributs étendus (champs personnalisés) associées à un projet. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Obtient ou définit une valeur de ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Obtient ou définit une valeur de FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Obtient ou définit une valeur indiquant si FiscalYearStart est défini ou non. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Obtient ou définit une valeur de FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Obtient ou définit les paramètres de mondialisation (spécifiques à la langue) du projet. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Obtient ou définit une valeur de Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Obtient ou définit une valeur indiquant si HonorConstraints est défini ou non. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Obtient ou définit une valeur de HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Obtient ou définit une valeur indiquant si InsertedProjectsLikeSummary est défini ou non. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Obtient ou définit une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Obtient ou définit une valeur de Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Obtient ou définit une valeur de LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Obtient ou définit une valeur de LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Obtient ou définit une valeur de LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Obtient ou définit une valeur de Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Obtient ou définit une valeur indiquant si MicrosoftProjectServerURL est défini ou non. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Obtient ou définit une valeur de MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Obtient ou définit une valeur de MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Obtient ou définit une valeur indiquant si MoveCompletedEndsBack est défini ou non. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Obtient ou définit une valeur indiquant si MoveCompletedEndsForward est défini ou non. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Obtient ou définit une valeur indiquant si MoveRemainingStartsBack est défini ou non. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Obtient ou définit une valeur indiquant si MoveRemainingStartsForward est défini ou non. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Obtient ou définit une valeur indiquant si MultipleCriticalPaths est défini ou non. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Obtient ou définit une valeur de Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Obtient ou définit une valeur indiquant si NewTasksAreManual est défini ou non. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Obtient ou définit une valeur indiquant si NewTasksEffortDriven est défini ou non. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Obtient ou définit une valeur indiquant si NewTasksEstimated est défini ou non. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Obtient ou définit une valeur de NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Obtient une collection contenant les instances de la classe [`OleObject`](../oleobject/) qui sont liées ou incorporées à ce fichier de projet. Disponible uniquement pour le format de fichier mpp. Cette collection est en lecture seule, sauf pour l'opération 'Clear'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Obtient l'objet OutlineCodeDefinitionCollection. La collection des définitions de codes de plan associés à un projet. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Obtient un objet contenant les propriétés spécifiques à Primavera pour un projet lu à partir d'un fichier Primavera. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Obtient ou définit une valeur indiquant si ProjectExternallyEdited est défini ou non. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Obtient ou définit une valeur indiquant si RemoveFileProperties est défini ou non. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Obtient l'objet ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Obtient toutes les définitions de filtres basés sur les ressources. ResourceFilters est une collection d'objets [`Filter`](../filter/). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Obtient toutes les définitions de groupes basés sur les ressources. ResourceGroups est une collection d'objets [`Group`](../group/). |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Obtient l'objet ResourceCollection. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Obtient ou définit une valeur de Revision. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Obtient la racine de l'arbre des tâches. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Obtient ou définit une valeur de SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Obtient ou définit une valeur indiquant si ScheduleFromStart est défini ou non. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Obtient ou définit une valeur indiquant si ShowProjectSummaryTask est défini ou non. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Obtient ou définit une valeur indiquant si SplitsInProgressTasks est défini ou non. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Obtient ou définit une valeur indiquant si SpreadActualCost est défini ou non. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Obtient ou définit une valeur indiquant si SpreadPercentComplete est défini ou non. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Obtient ou définit une valeur de StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Obtient ou définit une valeur de StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Obtient ou définit une valeur de Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Obtient une liste d'objets [`Table`](../table/). |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Obtient toutes les définitions de filtres basées sur les tâches. TaskFilters est une collection d'objets [`Filter`](../filter/). |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Obtient toutes les définitions de groupes basées sur les tâches. TaskGroups est une collection d'objets [`Group`](../group/). |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Obtient l'objet [`TaskLinkCollection`](../tasklinkcollection/). |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Obtient ou définit une valeur indiquant si TaskUpdatesResource est défini ou non. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Obtient ou définit une valeur de Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Obtient ou définit une valeur de TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Obtient ou définit une valeur de TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Obtient ou définit une valeur de Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Obtient ou définit une valeur de Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Obtient ou définit une valeur indiquant si UpdateManuallyScheduledTasksWhenEditingLinks est défini ou non. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Obtient une instance de la classe [`VbaProject`](./vbaproject/). |
| [Views](../../aspose.tasks/project/views/) { get; } | Obtient une liste d'objets [`View`](../view/). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Obtient ou définit la définition du code WBS pour le projet. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Obtient ou définit une valeur de WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Obtient ou définit une valeur de WorkFormat. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Copie les données principales et les propriétés du projet vers un autre projet. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Copie les données principales et les propriétés du projet vers un autre projet. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Énumère récursivement toutes les tâches du projet, y compris la tâche racine. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Renvoie le temps d’enregistrement de la ligne de base. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Obtient l’objet [`Duration`](../duration/) avec le nombre spécifié d’unités et le format de durée par défaut qui est défini dans les paramètres du projet [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Obtient l’objet [`Duration`](../duration/) avec le nombre spécifié d’unités [`TimeUnitType`](../timeunittype/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Obtient l’objet [`Duration`](../duration/) avec la valeur TimeSpan spécifiée et la valeur [`TimeUnitType`](../timeunittype/) spécifiée. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/) par défaut (Jours). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/) par défaut (Jours) et le [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) fourni |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Renvoie le nombre de pages du projet à rendre en utilisant les [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) fournis. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/) fourni. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/) et le [`PageSize`](../../aspose.tasks.visualization/pagesize/) fournis. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/) et le [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) fournis. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Renvoie le nombre de pages du projet à rendre en utilisant le [`Timescale`](../../aspose.tasks.visualization/timescale/), le [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) et la plage de dates. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Renvoie une collection de liens de tâches qui sont les prédécesseurs de la tâche spécifiée. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Obtient l’objet [`Duration`](../duration/) avec la valeur Double spécifiée et le format de travail par défaut. |
| [Print](../../aspose.tasks/project/print/#print)() | Imprime le projet sur l’imprimante par défaut avec les paramètres d’imprimante par défaut en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Imprime le projet selon les paramètres d’imprimante spécifiés en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Imprime le projet sur l’imprimante par défaut avec les paramètres d’imprimante par défaut et des options d’enregistrement personnalisées en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Imprime le projet sur l’imprimante spécifiée avec les paramètres d’imprimante par défaut en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Imprime le projet selon les paramètres d’imprimante spécifiés et des options d’enregistrement personnalisées en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Imprime le projet selon les paramètres d’imprimante spécifiés en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Imprime le projet selon les paramètres d’imprimante spécifiés, des options d’enregistrement personnalisées et le nom de document spécifié en utilisant le contrôleur d’impression standard (sans interface utilisateur). |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Replanifie les identifiants, les niveaux d’outline, les dates de début/fin de toutes les tâches du projet, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Replanifie les identifiants, les niveaux d’outline, les dates de début/fin de toutes les tâches du projet, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût avec une validation facultative. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Recalcule l’identifiant, le début et la fin des ressources. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Élimine les affectations de ressources invalides de la liste des affectations de ressources du projet. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Renuméroter le code WBS de toutes les tâches. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Renuméroter le code WBS des tâches passées. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Replanifie le travail de projet non terminé pour commencer après une date spécifiée. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Replanifie le travail non terminé d’une liste de tâches spécifiée pour commencer après une date spécifiée. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Enregistre les données du projet dans le fichier au format mpp. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Enregistre les données du projet dans le flux. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Enregistre le projet dans un flux en utilisant les options d’enregistrement spécifiées. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Enregistre les données du projet dans le fichier. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Enregistre le document dans un fichier en utilisant les options d’enregistrement spécifiées. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Enregistre le projet en tant que modèle dans un flux spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Enregistre le projet en tant que modèle dans le chemin de fichier spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Enregistre le projet en tant que modèle dans un flux spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Enregistre le projet en tant que modèle. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Enregistre le rapport d’aperçu du projet dans le flux. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Enregistre le rapport d’aperçu du projet dans un fichier PDF. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Enregistre le rapport du projet du type spécifié dans le flux spécifié. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Enregistre le rapport du projet du type spécifié au format PDF dans le chemin de fichier spécifié. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Collecte récursivement toutes les sous‑tâches de la tâche racine. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Enregistre les champs de base de référence dans la base de référence spécifiée pour l’ensemble du projet. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Enregistre les champs de base de référence dans la base de référence spécifiée pour les tâches sélectionnées. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Définit l’heure d’enregistrement de la base de référence. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Marque tout le travail comme terminé jusqu’à une date spécifiée pour l’ensemble du projet. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Marque tout le travail comme terminé jusqu’à une date spécifiée pour la liste de tâches spécifiée. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Obtient les informations du fichier de projet depuis le flux. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Lit les informations du fichier de projet depuis le fichier. |

## Remarques

Le **Project** est une classe centrale dans la bibliothèque Aspose.Tasks.

On peut utiliser **Project** pour lire l'un des formats de gestion de projet pris en charge : MPP, MPT, MPX, XML.

Pour charger un document existant dans l'un des formats pris en charge, transmettez un nom de fichier ou un flux à l'un des constructeurs **Project**. Pour créer un projet vierge, appelez le constructeur sans paramètres.

Utilisez l'une des surcharges de la méthode Save pour enregistrer le projet dans l'un des formats [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) : Primavera : P6 XML, PM XER ; Microsoft Excel : XLSX, XML ; Mise en page fixe : PDF ; Images : JPEG, PNG, BMP, TIFF, SVG ; Texte : TXT ; Autres : HTML.

Le **Project** stocke les informations globales du projet telles que [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), et [`ExtendedAttributes`](./extendedattributes/). La plupart de ces objets sont accessibles via les propriétés correspondantes de la classe **Project**.

Le **Project** est une entité racine qui contient des points d'entrée pour manipuler d'autres entités du projet, telles que [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) et [`Calendar`](../calendar/).

Les entités **Project** peuvent être accessibles via des collections typées, par exemple [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), etc.

## Exemples

Montre comment travailler avec une instance &lt;see cref="Aspose.Tasks.Project"/&gt;.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// ajout de nouvelles tâches et définition des propriétés souhaitées
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// ajout de nouvelles ressources
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// ajout de nouvelles affectations de ressources
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// enregistrer le projet dans l'un des formats disponibles
// ici nous l'enregistrons au format de fichier XML Microsoft Project.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


