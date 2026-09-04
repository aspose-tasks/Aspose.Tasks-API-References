---
title: "Projet"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un projet."
type: docs
weight: 220
url: /fr/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

Représente un projet.

--------------------

La **Project** est une classe centrale dans la bibliothèque Aspose.Tasks.

On peut utiliser **Project** pour lire l'un des formats de gestion de projet pris en charge : MPP, MPT, MPX, XML.

Pour charger un document existant dans l'un des formats pris en charge, transmettez un nom de fichier ou un flux à l'un des constructeurs de **Project**. Pour créer un projet vierge, appelez le constructeur sans paramètres.

Utilisez l'une des surcharges de la méthode Save pour enregistrer le projet dans l'un des formats [SaveFileFormat](../../com.aspose.tasks/savefileformat) : Primavera : P6 XML, PM XER ; Microsoft Excel : XLSX, XML ; Mise en page fixe : PDF ; Images : JPEG, PNG, BMP, TIFF, SVG ; Texte : TXT ; Autres : HTML.

Pour imprimer le projet, utilisez l'une des surcharges de la méthode [print()](../../com.aspose.tasks/project\#print--).

Le **Project** stocke les informations globales du projet telles que `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)), `Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/ [setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)), `Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/ [setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), et `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/ [setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). La plupart de ces objets sont accessibles via les propriétés correspondantes de la classe **Project**.

Le **Project** est une entité racine qui contient des points d'entrée pour manipuler d'autres entités du projet, telles que [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) et [Calendar](../../com.aspose.tasks/calendar).

Les entités **Project** peuvent être accessibles via des collections typées, par exemple `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/ [Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)), `Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/ [setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)), `Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/ [setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), etc.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Project()](#Project--) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project). |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle protégé par mot de passe (fichier mpp ou mpt existant). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir du flux avec l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un flux. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) pour lire les données d'une base de données spécifiée par l'instance de la classe [DbSettings](../../com.aspose.tasks/dbsettings). |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir du flux avec l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Copie les données principales et les propriétés du projet vers un autre projet. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Copie les données principales et les propriétés du projet vers un autre projet. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Énumère récursivement toutes les tâches du projet, y compris la tâche racine. |
| [getActualsInSync()](#getActualsInSync--) | Obtient une valeur indiquant si ActualsInSync est défini ou non. |
| [getAdminProject()](#getAdminProject--) | Obtient une valeur indiquant si AdminProject est défini ou non. |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | Obtient une valeur indiquant si AreEditableActualCosts est défini ou non. |
| [getAuthor()](#getAuthor--) | Obtient la valeur de Author. |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | Obtient une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non. |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | Obtient si le coût d'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les taux des ressources. |
| [getAutolink()](#getAutolink--) | Obtient une valeur indiquant si Autolink est défini ou non. |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | Obtient la valeur de BaselineForEarnedValue. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Renvoie le moment d'enregistrement de la ligne de base. |
| [getBuiltInProps()](#getBuiltInProps--) | Obtient la collection des propriétés intégrées du projet. |
| [getCalculationMode()](#getCalculationMode--) | Obtient le mode de calcul d'un projet. |
| [getCalendar()](#getCalendar--) | Obtient une valeur de Calendar. |
| [getCalendars()](#getCalendars--) | Obtient l'objet [CalendarCollection](../../com.aspose.tasks/calendarcollection) de cette instance de Project. |
| [getCategory()](#getCategory--) | Obtient la valeur de Category. |
| [getComments()](#getComments--) | Obtient la valeur de Comments. |
| [getCompany()](#getCompany--) | Obtient la valeur de Company. |
| [getCreationDate()](#getCreationDate--) | Obtient la valeur de CreationDate. |
| [getCriticalPath()](#getCriticalPath--) | Obtient une collection contenant une liste de tâches Critiques qui composent le Chemin Critique de ce projet. |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | Les tâches sont considérées critiques par MS Project si le flottement total est inférieur ou égal à ce nombre de jours. |
| [getCurrencyCode()](#getCurrencyCode--) | Obtient la valeur de CurrencyCode. |
| [getCurrencyDigits()](#getCurrencyDigits--) | Obtient une valeur de CurrencyDigits. |
| [getCurrencySymbol()](#getCurrencySymbol--) | Obtient une valeur de CurrencySymbol. |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | Obtient une valeur de CurrencySymbolPosition. |
| [getCurrentDate()](#getCurrentDate--) | Obtient une valeur de CurrentDate. |
| [getCustomDateFormat()](#getCustomDateFormat--) | Obtient une valeur de CustomDateFormat. |
| [getCustomProps()](#getCustomProps--) | Obtient la collection des propriétés personnalisées du projet. |
| [getDateFormat()](#getDateFormat--) | Obtient une valeur de DateFormat. |
| [getDaysPerMonth()](#getDaysPerMonth--) | Obtient une valeur de DaysPerMonth. |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | Obtient une valeur de DefaultFinishTime. |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | Obtient une valeur de DefaultFixedCostAccrual. |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | Obtient une valeur de DefaultOvertimeRate. |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | Obtient une valeur de DefaultStandardRate. |
| [getDefaultStartTime()](#getDefaultStartTime--) | Obtient une valeur de DefaultStartTime. |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | Obtient une valeur de DefaultTaskEVMethod. |
| [getDefaultTaskType()](#getDefaultTaskType--) | Obtient une valeur de DefaultTaskType. |
| [getDefaultView()](#getDefaultView--) | Obtient la vue par défaut du projet. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Obtient l'instance de la classe [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) qui représente une collection des jours ouvrables hebdomadaires et des heures de travail par défaut du projet. |
| [getDisplayOptions()](#getDisplayOptions--) | Obtient une instance de la classe [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions). |
| [getDuration(double val)](#getDuration-double-) | Obtient l'objet [Duration](../../com.aspose.tasks/duration) avec le nombre spécifié d'unités et le format de durée par défaut qui est défini dans les paramètres du projet [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | Obtient l'objet [Duration](../../com.aspose.tasks/duration) avec le nombre spécifié d'unités [TimeUnitType](../../com.aspose.tasks/timeunittype). |
| [getDurationFormat()](#getDurationFormat--) | Obtient une valeur de DurationFormat. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Obtient une valeur de EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtient l'objet ExtendedAttributeDefinitionCollection. |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | Obtient une valeur de ExtendedCreationDate. |
| [getFinishDate()](#getFinishDate--) | Obtient une valeur de FinishDate. |
| [getFiscalYearStart()](#getFiscalYearStart--) | Obtient une valeur indiquant si FiscalYearStart est défini ou non. |
| [getFyStartDate()](#getFyStartDate--) | Obtient une valeur de FyStartDate. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Obtient les paramètres de mondialisation (spécifiques à la langue) du projet. |
| [getGuid()](#getGuid--) | Obtient une valeur de Guid. |
| [getHonorConstraints()](#getHonorConstraints--) | Obtient une valeur indiquant si HonorConstraints est défini ou non. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Obtient une valeur de HyperlinkBase. |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | Obtient une valeur indiquant si InsertedProjectsLikeSummary est défini ou non. |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | Obtient une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non. |
| [getKeywords()](#getKeywords--) | Obtient une valeur de Keywords. |
| [getLastAuthor()](#getLastAuthor--) | Obtient une valeur de LastAuthor. |
| [getLastPrinted()](#getLastPrinted--) | Obtient une valeur de LastPrinted. |
| [getLastSaved()](#getLastSaved--) | Obtient une valeur de LastSaved. |
| [getManager()](#getManager--) | Obtient une valeur de Manager. |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | Obtient une valeur indiquant si MicrosoftProjectServerURL est défini ou non. |
| [getMinutesPerDay()](#getMinutesPerDay--) | Obtient une valeur de MinutesPerDay. |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | Obtient une valeur de MinutesPerWeek. |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | Obtient une valeur indiquant si MoveCompletedEndsBack est défini ou non. |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | Obtient une valeur indiquant si MoveCompletedEndsForward est défini ou non. |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | Obtient une valeur indiquant si MoveRemainingStartsBack est défini ou non. |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | Obtient une valeur indiquant si MoveRemainingStartsForward est défini ou non. |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | Obtient une valeur indiquant si MultipleCriticalPaths est défini ou non. |
| [getName()](#getName--) | Obtient une valeur de Name. |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | Obtient une valeur de NewTaskStartDate. |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | Obtient une valeur indiquant si NewTasksAreManual est défini ou non. |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | Obtient une valeur indiquant si NewTasksEffortDriven est défini ou non. |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | Obtient une valeur indiquant si NewTasksEstimated est défini ou non. |
| [getOleObjects()](#getOleObjects--) | Obtient une collection contenant les instances de la classe [OleObject](../../com.aspose/tasks/oleobject) qui sont liées ou incorporées à ce fichier de projet. |
| [getOutlineCodes()](#getOutlineCodes--) | Obtient l'objet OutlineCodeDefinitionCollection. |
| [getPageCount()](#getPageCount--) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) par défaut (Jours). |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Renvoie le nombre de pages pour le projet à rendre en utilisant les [SaveOptions](../../com.aspose.tasks/saveoptions) fournis. |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) et le [PresentationFormat](../../com.aspose.tasks/presentationformat) fournis. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) et le [PageSize](../../com.aspose.tasks/pagesize) fournis. |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale), le [PresentationFormat](../../com.aspose.tasks/presentationformat) et la plage de dates fournis. |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) par défaut (Jours) et le [PresentationFormat](../../com.aspose.tasks/presentationformat) fourni. |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) fourni. |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Renvoie une collection de liens de tâches qui sont les prédécesseurs de la tâche spécifiée. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Obtient un objet contenant les propriétés spécifiques à Primavera pour un projet lu à partir d'un fichier Primavera. |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | Obtient une valeur indiquant si ProjectExternallyEdited est défini ou non. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Obtient les informations du fichier de projet depuis le flux. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Lit les informations du fichier de projet depuis le fichier. |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | Obtient une valeur indiquant si RemoveFileProperties est défini ou non. |
| [getResourceAssignments()](#getResourceAssignments--) | Obtient l'objet ResourceAssignmentCollection. |
| [getResourceFilters()](#getResourceFilters--) | Obtient toutes les définitions de filtres basées sur les ressources. |
| [getResourceGroups()](#getResourceGroups--) | Obtient toutes les définitions de groupes basées sur les ressources. |
| [getResources()](#getResources--) | Obtient l'objet ResourceCollection. |
| [getRevision()](#getRevision--) | Obtient une valeur de Revision. |
| [getRootTask()](#getRootTask--) | Obtient la racine de l'arbre des tâches. |
| [getSaveVersion()](#getSaveVersion--) | Obtient une valeur de SaveVersion. |
| [getScheduleFromStart()](#getScheduleFromStart--) | Obtient une valeur indiquant si ScheduleFromStart est défini ou non. |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | Obtient une valeur indiquant si ShowProjectSummaryTask est défini ou non. |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | Obtient une valeur indiquant si SplitsInProgressTasks est défini ou non. |
| [getSpreadActualCost()](#getSpreadActualCost--) | Obtient une valeur indiquant si SpreadActualCost est défini ou non. |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | Obtient une valeur indiquant si SpreadPercentComplete est défini ou non. |
| [getStartDate()](#getStartDate--) | Obtient une valeur de StartDate. |
| [getStatusDate()](#getStatusDate--) | Obtient une valeur de StatusDate. |
| [getSubject()](#getSubject--) | Obtient une valeur de Subject. |
| [getTables()](#getTables--) | Obtient une liste d'objets [Table](../../com.aspose.tasks/table). |
| [getTaskFilters()](#getTaskFilters--) | Obtient toutes les définitions de filtres basées sur les tâches. |
| [getTaskGroups()](#getTaskGroups--) | Obtient toutes les définitions de groupes basées sur les tâches. |
| [getTaskLinks()](#getTaskLinks--) | Obtient l'objet [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection). |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | Obtient une valeur indiquant si TaskUpdatesResource est défini ou non. |
| [getTemplate()](#getTemplate--) | Obtient une valeur de Template. |
| [getTimescaleFinish()](#getTimescaleFinish--) | Obtient une valeur de TimescaleFinish. |
| [getTimescaleStart()](#getTimescaleStart--) | Obtient une valeur de TimescaleStart. |
| [getTitle()](#getTitle--) | Obtient une valeur de Title. |
| [getUid()](#getUid--) | Obtient la valeur de Uid. |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | Obtient une valeur indiquant si UpdateManuallyScheduledTasksWhenEditingLinks est défini ou non. |
| [getVbaProject()](#getVbaProject--) | Obtient une instance de la classe `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)). |
| [getViews()](#getViews--) | Obtient une liste d'objets [View](../../com.aspose.tasks/view). |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Obtient la définition du code WBS pour le projet. |
| [getWeekStartDay()](#getWeekStartDay--) | Obtient une valeur de WeekStartDay. |
| [getWork(double val)](#getWork-double-) | Obtient l'objet [Duration](../../com.aspose.tasks/duration) avec la valeur `double` spécifiée et le format de travail par défaut. |
| [getWorkFormat()](#getWorkFormat--) | Obtient une valeur de WorkFormat. |
| [print()](#print--) | Imprime le projet sur l'imprimante par défaut avec les paramètres d'imprimante par défaut en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Imprime le projet sur l'imprimante par défaut avec les paramètres d'imprimante par défaut et des options d'enregistrement personnalisées en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Imprime le projet selon les paramètres d'imprimante spécifiés en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Imprime le projet selon les paramètres d'imprimante spécifiés et des options d'enregistrement personnalisées en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Imprime le projet selon les paramètres d'imprimante spécifiés, des options d'enregistrement personnalisées et le nom de document spécifié en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Imprime le projet selon les paramètres d'imprimante spécifiés en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [print(String printerName)](#print-java.lang.String-) | Imprime le projet sur l'imprimante spécifiée avec les paramètres d'imprimante par défaut en utilisant le contrôleur d'impression standard (sans interface utilisateur). |
| [recalculate()](#recalculate--) | Replanifie les identifiants de toutes les tâches du projet, les niveaux de plan, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Replanifie les identifiants de toutes les tâches du projet, les niveaux de plan, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût avec validation facultative. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Recalcule l'identifiant, le début et la fin des ressources. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Recalcule le début et la fin des ressources. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Élimine les affectations de ressources invalides de la liste des affectations de ressources du projet. |
| [renumberWBSCode()](#renumberWBSCode--) | Renumérote le code WBS de toutes les tâches. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Renumérote le code WBS des tâches transmises. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Replanifie le travail de projet incomplet pour commencer après une date spécifiée. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Replanifie le travail incomplet d'une liste spécifiée de tâches pour commencer après une date spécifiée. |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | Enregistre le projet dans un flux en utilisant les options d'enregistrement spécifiées. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Enregistre les données du projet dans le flux. |
| [save(String filename)](#save-java.lang.String-) | Enregistre les données du projet dans le fichier au format mpp. |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | Enregistre le document dans un fichier en utilisant les options d'enregistrement spécifiées. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Enregistre les données du projet dans le fichier. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Enregistre le projet comme modèle dans un flux spécifié. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Enregistre le projet comme modèle dans un flux spécifié. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Enregistre le projet comme modèle dans le chemin de fichier spécifié. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Enregistre le projet comme modèle. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Enregistre le rapport d'aperçu du projet dans le flux. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Enregistre le rapport du projet du type spécifié dans le flux spécifié. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Enregistre le rapport d'aperçu du projet dans un fichier PDF. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Enregistre le rapport du projet du type spécifié au format PDF dans le chemin de fichier spécifié. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Collecte récursivement toutes les sous‑tâches de la tâche racine. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si ActualsInSync est défini ou non. |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si AdminProject est défini ou non. |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si AreEditableActualCosts est défini ou non. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit la valeur de Author. |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non. |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | Définit si le coût de l'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les taux des ressources. |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si Autolink est défini ou non. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Enregistre les champs de référence dans la référence spécifiée pour l'ensemble du projet. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Enregistre les champs de référence dans la référence spécifiée pour les tâches sélectionnées. |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | Définit la valeur de BaselineForEarnedValue. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Définit l'heure d'enregistrement de la référence. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Définit le mode de calcul d'un projet. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Définit une valeur de Calendar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Définit la valeur de Category. |
| [setComments(String value)](#setComments-java.lang.String-) | Définit la valeur de Comments. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Définit la valeur de Company. |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | Définit la valeur de CreationDate. |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | Les tâches sont considérées critiques par MS Project si le flottement total est inférieur ou égal à ce nombre de jours. |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | Définit la valeur de CurrencyCode. |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | Définit la valeur de CurrencyDigits. |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | Définit la valeur de CurrencySymbol. |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | Définit la valeur de CurrencySymbolPosition. |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | Définit la valeur de CurrentDate. |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | Définit la valeur de CustomDateFormat. |
| [setDateFormat(int value)](#setDateFormat-int-) | Définit la valeur de DateFormat. |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | Définit la valeur de DaysPerMonth. |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | Définit la valeur de DefaultFinishTime. |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | Définit la valeur de DefaultFixedCostAccrual. |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | Définit la valeur de DefaultOvertimeRate. |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | Définit une valeur de DefaultStandardRate. |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | Définit une valeur de DefaultStartTime. |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | Définit une valeur de DefaultTaskEVMethod. |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | Définit une valeur de DefaultTaskType. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Définit la vue par défaut du projet. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Définit une valeur de DurationFormat. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Définit une valeur de EarnedValueMethod. |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | Définit une valeur de ExtendedCreationDate. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Définit une valeur de FinishDate. |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si FiscalYearStart est défini ou non. |
| [setFyStartDate(int value)](#setFyStartDate-int-) | Définit une valeur de FyStartDate. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | Définit les paramètres de mondialisation (spécifiques à la langue) du projet. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Définit une valeur de Guid. |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si HonorConstraints est défini ou non. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Définit une valeur de HyperlinkBase. |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si InsertedProjectsLikeSummary est défini ou non. |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Définit une valeur de Keywords. |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | Définit une valeur de LastAuthor. |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | Définit une valeur de LastPrinted. |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | Définit une valeur de LastSaved. |
| [setManager(String value)](#setManager-java.lang.String-) | Définit une valeur de Manager. |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MicrosoftProjectServerURL est défini ou non. |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | Définit une valeur de MinutesPerDay. |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | Définit une valeur de MinutesPerWeek. |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MoveCompletedEndsBack est défini ou non. |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MoveCompletedEndsForward est défini ou non. |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MoveRemainingStartsBack est défini ou non. |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MoveRemainingStartsForward est défini ou non. |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si MultipleCriticalPaths est défini ou non. |
| [setName(String value)](#setName-java.lang.String-) | Définit une valeur de Name. |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | Définit une valeur de NewTaskStartDate. |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si NewTasksAreManual est défini ou non. |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si NewTasksEffortDriven est défini ou non. |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si NewTasksEstimated est défini ou non. |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si ProjectExternallyEdited est défini ou non. |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si RemoveFileProperties est défini ou non. |
| [setRevision(int value)](#setRevision-int-) | Définit une valeur de Revision. |
| [setSaveVersion(int value)](#setSaveVersion-int-) | Définit une valeur de SaveVersion. |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si ScheduleFromStart est défini ou non. |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | Définit une valeur indiquant si ShowProjectSummaryTask est défini ou non. |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si SplitsInProgressTasks est défini ou non. |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si SpreadActualCost est défini ou non. |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si SpreadPercentComplete est défini ou non. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Définit une valeur de StartDate. |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | Définit une valeur de StatusDate. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Définit une valeur de Subject. |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si TaskUpdatesResource est défini ou non. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Définit une valeur de Template. |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | Définit une valeur de TimescaleFinish. |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | Définit une valeur de TimescaleStart. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Définit une valeur de Title. |
| [setUid(String value)](#setUid-java.lang.String-) | Définit une valeur de Uid. |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si UpdateManuallyScheduledTasksWhenEditingLinks est défini ou non. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Définit la définition du code WBS pour le projet. |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | Définit une valeur pour WeekStartDay. |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | Définit une valeur pour WorkFormat. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour l'ensemble du projet. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour la liste de tâches spécifiée. |
### Project() {#Project--}
```
public Project()
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project).

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle protégé par mot de passe (fichier mpp ou mpt existant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Chemin vers le modèle à partir duquel créer le projet. |
|  | protectionPassword | java.lang.String | Mot de passe de protection. |

--------------------

La lecture des fichiers protégés par mot de passe est actuellement prise en charge uniquement pour le format de fichier MSP 2003. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Chemin vers le modèle à partir duquel créer le projet. |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir du flux avec l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Flux du projet java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) qui permet de personnaliser la lecture des formats Primavera (XER ou XML). |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Chemin vers le modèle à partir duquel créer le projet. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | la méthode de rappel spécifiée pour gérer les erreurs d'analyse XML. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream pour charger un modèle depuis. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Chemin vers le modèle à partir duquel créer le projet |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | l'instance spécifiée de la classe [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions). |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) pour lire les données d'une base de données spécifiée par l'instance de la classe [DbSettings](../../com.aspose.tasks/dbsettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | l'instance spécifiée de la classe [DbSettings](../../com.aspose.tasks/dbsettings). |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream pour charger un modèle depuis. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | la méthode de rappel spécifiée pour gérer les erreurs d'analyse XML. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream pour charger un modèle depuis. |
|  | protectionPassword | java.lang.String | Mot de passe de protection. |

--------------------

La lecture des fichiers protégés par mot de passe est actuellement prise en charge uniquement pour le format de fichier MSP 2003. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Chemin vers le modèle à partir duquel créer le projet |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions). |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Initialise une nouvelle instance de la classe [Project](../../com.aspose.tasks/project) à partir du flux avec l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Flux du projet java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | l'instance spécifiée de la classe [LoadOptions](../../com.aspose.tasks/loadoptions) |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Prj](../../com.aspose.tasks/prj) pour obtenir la clé de propriété. |

**Returns:**
T - la valeur à laquelle la propriété est mappée dans ce conteneur.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Prj](../../com.aspose.tasks/prj) pour obtenir la clé de propriété. |
| val | T | la valeur. |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Copie les données principales et les propriétés du projet vers un autre projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Un autre projet vers lequel copier les données. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Copie les données principales et les propriétés du projet vers un autre projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Un autre projet vers lequel copier les données. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Options de copie pour contrôler le processus de copie. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Énumère récursivement toutes les tâches du projet, y compris la tâche racine.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable qui peut être utilisé pour parcourir toutes les tâches du projet.

--------------------

Fournit une méthode plus légère pour parcourir les tâches comparée à la méthode [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) car elle n’alloue pas de mémoire pour toutes les tâches.
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


Obtient une valeur indiquant si ActualsInSync est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


Obtient une valeur indiquant si AdminProject est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


Obtient une valeur indiquant si AreEditableActualCosts est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Obtient la valeur de Author.

**Returns:**
java.lang.String - une valeur de Author.
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


Obtient une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


Obtient si le coût d'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les taux des ressources.

**Returns:**
boolean - indique si le coût de l'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les tarifs des ressources.
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Obtient une valeur indiquant si Autolink est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


Obtient la valeur de BaselineForEarnedValue.

**Returns:**
int - une valeur de BaselineForEarnedValue.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Renvoie l'heure d'enregistrement de la ligne de base. Renvoie DateTime.MinValue (00:00:00.0000000 UTC, 1er janvier 0001) si la ligne de base n'a pas été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baselineNumber | int | Le numéro de la ligne de base [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - La date et l'heure du dernier enregistrement de la ligne de base.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Obtient la collection des propriétés intégrées du projet.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Obtient le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)).

**Returns:**
int - mode de calcul d'un projet.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Obtient une valeur de Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Obtient l'objet [CalendarCollection](../../com.aspose.tasks/calendarcollection) de cette instance de Project.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Obtient la valeur de Category.

**Returns:**
java.lang.String - une valeur de Category.
### getComments() {#getComments--}
```
public final String getComments()
```


Obtient la valeur de Comments.

**Returns:**
java.lang.String - une valeur de Comments.
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Obtient la valeur de Company.

**Returns:**
java.lang.String - une valeur de Company.
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


Obtient la valeur de CreationDate.

**Returns:**
java.util.Date - une valeur de CreationDate.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Obtient une collection contenant une liste de tâches Critiques qui composent le Chemin Critique de ce projet.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

Ceci est une opération O(n), où n est le nombre de tâches dans le projet.
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


Les tâches sont considérées critiques par MS Project si le flottement total est inférieur ou égal à ce nombre de jours.

**Returns:**
int - la valeur maximale du temps de marge totale (en jours) à laquelle une tâche est considérée comme critique
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


Obtient la valeur de CurrencyCode.

**Returns:**
java.lang.String - une valeur de CurrencyCode.
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


Obtient une valeur de CurrencyDigits.

**Returns:**
int - une valeur de CurrencyDigits.
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


Obtient une valeur de CurrencySymbol.

**Returns:**
java.lang.String - une valeur de CurrencySymbol.
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


Obtient une valeur de CurrencySymbolPosition.

**Returns:**
int - une valeur de CurrencySymbolPosition.
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


Obtient une valeur de CurrentDate.

**Returns:**
java.util.Date - une valeur de CurrentDate.
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


Obtient une valeur de CustomDateFormat.

**Returns:**
java.lang.String - une valeur de CustomDateFormat.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Obtient la collection des propriétés personnalisées du projet.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Obtient une valeur de DateFormat.

**Returns:**
int - une valeur de DateFormat.
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


Obtient une valeur de DaysPerMonth.

**Returns:**
int - une valeur de DaysPerMonth.
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


Obtient une valeur de DefaultFinishTime.

**Returns:**
java.util.Date - une valeur de DefaultFinishTime.
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


Obtient une valeur de DefaultFixedCostAccrual.

**Returns:**
int - une valeur de DefaultFixedCostAccrual.
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


Obtient une valeur de DefaultOvertimeRate.

**Returns:**
double - une valeur de DefaultOvertimeRate.
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


Obtient une valeur de DefaultStandardRate.

**Returns:**
double - une valeur de DefaultStandardRate.
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


Obtient une valeur de DefaultStartTime.

**Returns:**
java.util.Date - une valeur de DefaultStartTime.
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


Obtient une valeur de DefaultTaskEVMethod.

**Returns:**
int - une valeur de DefaultTaskEVMethod.
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


Obtient une valeur de DefaultTaskType.

**Returns:**
int - une valeur de DefaultTaskType.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Obtient la vue par défaut du projet.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Obtient l'instance de la classe [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) qui représente une collection des jours ouvrables hebdomadaires et des heures de travail par défaut du projet.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

Les données ne se trouvent que dans les fichiers mpp (pas dans xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Obtient une instance de la classe [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions).

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Obtient l'objet [Duration](../../com.aspose.tasks/duration) avec le nombre spécifié d'unités et le format de durée par défaut qui est défini dans les paramètres du projet [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | val | double | nombre spécifié d'unités. |

--------------------

Cette méthode doit être utilisée avec précaution car elle renvoie des durées différentes selon le paramètre Project.DurationFormat. Par exemple, GetWork(1.0) renverra 1 heure lorsque Project.DurationFormat est TimeUnitType.Hour ou 1 jour si Project.DurationFormat est TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


Obtient l'objet [Duration](../../com.aspose.tasks/duration) avec le nombre spécifié d'unités [TimeUnitType](../../com.aspose.tasks/timeunittype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| val | double | nombre spécifié d'unités. |
| timeUnit | byte | valeur spécifiée de TimeUnitType. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Obtient une valeur de DurationFormat.

**Returns:**
byte - une valeur de DurationFormat.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Obtient une valeur de EarnedValueMethod.

**Returns:**
int - une valeur de EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Obtient l'objet ExtendedAttributeDefinitionCollection. La collection des définitions d'attributs étendus (champs personnalisés) associées à un projet.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


Obtient une valeur de ExtendedCreationDate.

**Returns:**
java.util.Date - une valeur de ExtendedCreationDate.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Obtient une valeur de FinishDate.

**Returns:**
java.util.Date - une valeur de FinishDate.
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


Obtient une valeur indiquant si FiscalYearStart est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


Obtient une valeur de FyStartDate.

**Returns:**
int - une valeur de FyStartDate.
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


Obtient les paramètres de mondialisation (spécifiques à la langue) du projet.

La méthode recommandée consiste à utiliser des littéraux ou des formats indépendants de la culture dans tout le projet. Cependant, si un projet utilise des littéraux spécifiques à une culture, cette classe peut être utilisée pour aider le moteur de calcul à analyser ces littéraux.

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtient une valeur de Guid.

**Returns:**
java.util.UUID - une valeur de Guid.
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


Obtient une valeur indiquant si HonorConstraints est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


Obtient une valeur de HyperlinkBase.

**Returns:**
java.lang.String - une valeur de HyperlinkBase.
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


Obtient une valeur indiquant si InsertedProjectsLikeSummary est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


Obtient une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Obtient une valeur de Keywords.

**Returns:**
java.lang.String - une valeur de Keywords.
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


Obtient une valeur de LastAuthor.

**Returns:**
java.lang.String - une valeur de LastAuthor.
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


Obtient une valeur de LastPrinted.

**Returns:**
java.util.Date - une valeur de LastPrinted.
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


Obtient une valeur de LastSaved.

**Returns:**
java.util.Date - une valeur de LastSaved.
### getManager() {#getManager--}
```
public final String getManager()
```


Obtient une valeur de Manager.

**Returns:**
java.lang.String - une valeur de Manager.
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


Obtient une valeur indiquant si MicrosoftProjectServerURL est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


Obtient une valeur de MinutesPerDay.

**Returns:**
int - une valeur de MinutesPerDay.
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


Obtient une valeur de MinutesPerWeek.

**Returns:**
int - une valeur de MinutesPerWeek.
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


Obtient une valeur indiquant si MoveCompletedEndsBack est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


Obtient une valeur indiquant si MoveCompletedEndsForward est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


Obtient une valeur indiquant si MoveRemainingStartsBack est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


Obtient une valeur indiquant si MoveRemainingStartsForward est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


Obtient une valeur indiquant si MultipleCriticalPaths est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Obtient une valeur de Name.

**Returns:**
java.lang.String - une valeur de Name.
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


Obtient une valeur de NewTaskStartDate.

**Returns:**
int - une valeur de NewTaskStartDate.
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


Obtient une valeur indiquant si NewTasksAreManual est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


Obtient une valeur indiquant si NewTasksEffortDriven est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


Obtient une valeur indiquant si NewTasksEstimated est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Obtient une collection contenant les instances de la classe [OleObject](../../com.aspose/tasks/oleobject) qui sont liées ou incorporées à ce fichier de projet.

--------------------

Disponible uniquement pour le format de fichier mpp. Cette collection est en lecture seule sauf pour l'opération 'Clear'.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Obtient l'objet OutlineCodeDefinitionCollection. La collection des définitions de code de plan associées à un projet.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Renvoie le nombre de pages pour le projet à rendre en utilisant le [Timescale](../../com.aspose.tasks/timescale) par défaut (Jours).

**Returns:**
int - Nombre de pages à rendre.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Renvoie le nombre de pages pour le projet à rendre en utilisant les [SaveOptions](../../com.aspose.tasks/saveoptions) fournis.

--------------------

&gt; ```
&gt; Dans cet exemple, l'instance de HtmlSaveOptions et le nombre de pages du HTML résultant sont écrits dans la console.
&gt; ``````

  [C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
public final int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
public final NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
public final boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
public final NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
public final NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
public final NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
public final Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
public final String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
public final NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
public final String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
public final Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
public final Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
public final String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
public final String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
public final NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
public final int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

