---
title: Project
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Représente un projet.
type: docs
weight: 1180
url: /fr/net/aspose.tasks/project/
---
## Project class

Représente un projet.

```csharp
public class Project
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Project](project#constructor)() | Initialise une nouvelle instance du[`Project`](../project) classe. |
| [Project](project#constructor_1)(DbSettings) | Initialise une nouvelle instance du[`Project`](../project) classe pour lire les données d'une base de données qui est spécifiée par l'instance de la[`DbSettings`](../../aspose.tasks.connectivity/dbsettings) classe. |
| [Project](project#constructor_2)(Stream) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un flux. |
| [Project](project#constructor_9)(StreamReader) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'une instance StreamReader. |
| [Project](project#constructor_10)(string) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Initialise une nouvelle instance du[`Project`](../project) classe du Stream avec l'instance spécifiée du[`LoadOptions`](../loadoptions) classe. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Initialise une nouvelle instance du[`Project`](../project) classe du Stream avec l'instance spécifiée du[`PrimaveraReadOptions`](../primaverareadoptions) classe. |
| [Project](project#constructor_8)(Stream, string) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project#constructor_11)(string, LoadOptions) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la[`LoadOptions`](../loadoptions) classe. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier mpp ou mpt existant). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée du[`PrimaveraReadOptions`](../primaverareadoptions) classe. |
| [Project](project#constructor_16)(string, string) | Initialise une nouvelle instance du[`Project`](../project) classe à partir d'un modèle protégé par mot de passe (fichier mpp ou mpt existant). |

## Propriétés

| Nom | La description |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Obtient la collection de propriétés intégrées du projet. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Obtient ou définit le mode de calcul d'un projet. Peut être l'une des valeurs de[`CalculationMode`](./calculationmode) énumération. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Obtient[`CalendarCollection`](../calendarcollection) objet de cette instance de projet. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Obtient une collection qui contient une liste de tâches critiques qui comprennent le chemin critique de ce projet. Il s'agit d'une opération O(n), où n est le nombre de tâches dans le projet. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Obtient la collection de propriétés personnalisées du projet. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Obtient ou définit la vue par défaut du projet. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Obtient l'instance de[`WeekDayCollection`](../weekdaycollection) classe qui représente une collection de jours ouvrables et d'heures de travail par défaut du projet. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Obtient une instance de[`ProjectDisplayOptions`](../projectdisplayoptions) classe. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Obtient l'objet ExtendedAttributeDefinitionCollection. La collection de définitions d'attributs étendus (champs personnalisés) associées à un projet. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Obtient une collection contenant les instances du[`OleObject`](../oleobject) classe qui sont liées ou incorporées à ce fichier de projet. Disponible uniquement pour le format de fichier mpp. Cette collection est en lecture seule, sauf pour l'opération "Effacer". |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Obtient l'objet OutlineCodeDefinitionCollection. La collection de définitions de code hiérarchique associées à un projet. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Obtient l'objet ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Obtient toutes les définitions de filtre basées sur les ressources. ResourceFilters est une collection de[`Filter`](../filter) objets. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Obtient toutes les définitions de groupes basés sur les ressources. ResourceGroups est une collection de[`Group`](../group) objets. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Obtient l'objet ResourceCollection. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Obtient la racine de l'arborescence des tâches. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Obtient une liste de[`Table`](../table) objets. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Obtient toutes les définitions de filtre basées sur les tâches. TaskFilters est une collection de[`Filter`](../filter) objets. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Obtient toutes les définitions de groupe basées sur les tâches. TaskGroups est une collection de[`Group`](../group) objets. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Obtient[`TaskLinkCollection`](../tasklinkcollection) objet. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Obtient une instance de[`VbaProject`](./vbaproject) classe. |
| [Views](../../aspose.tasks/project/views) { get; } | Obtient une liste de[`View`](../view) objets. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Obtient ou définit la définition de code WBS pour le projet. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Copie les principales données et propriétés du projet dans un autre projet. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Copie les principales données et propriétés du projet dans un autre projet. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Énumère de manière récursive toutes les tâches du projet, y compris la tâche racine. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Renvoie la durée de sauvegarde de référence. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Obtient[`Duration`](../duration) objet avec le nombre d'unités spécifié et le format de durée par défaut défini dans les paramètres du projet[`DurationFormat`](../prj/durationformat) . |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Obtient[`Duration`](../duration) objet avec le nombre spécifié de[`TimeUnitType`](../timeunittype) unités. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Obtient[`Duration`](../duration) objet avec le spécifiéTimeSpan valeur et spécifié[`TimeUnitType`](../timeunittype) valeur. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Renvoie le nombre de pages pour le projet à rendre en utilisant la valeur par défaut[`Timescale`](../../aspose.tasks.visualization/timescale) (Jours). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Renvoie le nombre de pages pour le projet à rendre en utilisant la valeur par défaut[`Timescale`](../../aspose.tasks.visualization/timescale) (Jours) et donné[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Renvoie le nombre de pages pour le projet à rendre en utilisant[`SaveOptions`](../../aspose.tasks.saving/saveoptions) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../aspose.tasks.visualization/timescale) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../aspose.tasks.visualization/timescale) et[`PageSize`](../../aspose.tasks.visualization/pagesize) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../aspose.tasks.visualization/timescale) et[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) . |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Renvoie le nombre de pages pour le projet à rendre en utilisant[`Timescale`](../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) et plage de dates. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Renvoie une collection de liens de tâches qui sont des prédécesseurs de la tâche spécifiée. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Obtient[`Duration`](../duration) objet avec le spécifiéDouble valeur et format de travail par défaut. |
| [Print](../../aspose.tasks/project/print#print)() | Imprime le projet sur l'imprimante par défaut avec les paramètres d'imprimante par défaut à l'aide du contrôleur d'impression standard (pas d'interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Imprime le projet selon les paramètres d'imprimante spécifiés à l'aide du contrôleur d'impression standard (pas d'interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Imprime le projet sur l'imprimante par défaut avec les paramètres d'imprimante par défaut et les options d'enregistrement personnalisées à l'aide du contrôleur d'impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Imprime le projet sur l'imprimante spécifiée avec les paramètres d'imprimante par défaut à l'aide du contrôleur d'impression standard (pas d'interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Imprime le projet en fonction des paramètres d'imprimante spécifiés et des options d'enregistrement personnalisées à l'aide du contrôleur d'impression standard (sans interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Imprime le projet selon les paramètres d'imprimante spécifiés à l'aide du contrôleur d'impression standard (pas d'interface utilisateur). |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Imprime le projet en fonction des paramètres d'imprimante spécifiés, des options d'enregistrement personnalisées et du nom de document spécifié à l'aide du contrôleur d'impression standard (sans interface utilisateur). |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Replanifie tous les identifiants de tâches du projet, les niveaux hiérarchiques, les dates de début/fin, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Replanifie tous les identifiants de tâches du projet, les niveaux hiérarchiques, les dates de début/fin, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût avec validation facultative. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Recalcule l'ID, le début et la fin des ressources. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Recalcule le début et la fin des ressources. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Élimine les affectations de ressources non valides de la liste des affectations de ressources du projet. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Renuméroter le code WBS de toutes les tâches. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Renuméroter le code WBS des tâches passées. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Replanifie les travaux de projet inachevés pour qu'ils commencent après une date spécifiée. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Replanifie le travail inachevé pour une liste spécifiée de tâches à démarrer après une date spécifiée. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Enregistre les données du projet dans le fichier au format mpp. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Enregistre le projet dans un flux à l'aide des options d'enregistrement spécifiées. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Enregistre les données du projet dans le flux. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Enregistre le projet dans un flux à l'aide des options d'enregistrement spécifiées. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Enregistre le document au format de fichier mpp en utilisant les options d'enregistrement spécifiées. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Enregistre les données du projet dans le fichier. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Enregistre le document dans un fichier à l'aide des options d'enregistrement spécifiées. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Enregistre le projet en tant que modèle dans un flux spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Enregistre le projet en tant que modèle dans le chemin de fichier spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Enregistre le projet en tant que modèle dans un flux spécifié. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Enregistre le projet en tant que modèle. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Enregistre le rapport de présentation du projet dans le flux. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Enregistre le rapport de synthèse du projet dans un fichier PDF. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Enregistre le rapport de projet du type spécifié dans le flux spécifié. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Enregistre le rapport de projet du type spécifié au format PDF dans le chemin de fichier spécifié. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Collecte de manière récursive toutes les tâches enfants de la tâche racine. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Enregistre les champs de ligne de base dans la ligne de base spécifiée pour l'ensemble du projet. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Enregistre les champs de ligne de base dans la ligne de base spécifiée pour les tâches sélectionnées. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Définit le temps de sauvegarde de base. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Met à jour tous les travaux comme terminés jusqu'à une date spécifiée pour l'ensemble du projet. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Met à jour tous les travaux comme terminés jusqu'à une date spécifiée pour la liste de tâches spécifiée. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Obtient les informations sur le fichier de projet à partir du flux. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Lire les informations de fichier de projet à partir du fichier. |

### Remarques

La **Projet** est une classe centrale dans la bibliothèque Aspose.Tasks.

On peut utiliser **Projet** pour lire l'un des formats de gestion de projet pris en charge : MPP, MPT, MPX, XML.

Pour charger un document existant dans l'un des formats pris en charge, transmettez un nom de fichier ou un flux dans l'un des **Projet** constructeurs. Pour créer un projet vide, appelez le constructeur sans paramètre.

Utilisez l'une des surcharges de méthode Save pour enregistrer le projet dans l'un des[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) formats : Primavera : P6 XML, PM XER ; Microsoft Excel : XLSX, XML ; Mise en page fixe : PDF ; Images : JPEG, PNG, BMP, TIFF, SVG ; Texte : TXT ; Autres : HTML.

Pour imprimer le projet, utilisez l'un des[`Print`](./print) surcharges de méthode.

La **Projet** stocke des informations à l'échelle du projet telles que[`Views`](./views) , [`BuiltInProps`](./builtinprops) ,[`CustomProps`](./customprops) , et[`ExtendedAttributes`](./extendedattributes) . La plupart de ces objets sont accessibles via les propriétés correspondantes du **Projet** classer.

La **Projet** est une entité racine qui contient des points d'entrée pour manipuler d'autres entités de projet, telles que[`Task`](../task) ,[`Resource`](../resource) ,[`ResourceAssignment`](../resourceassignment) ,[`ExtendedAttribute`](../extendedattribute) et[`Calendar`](../calendar).

Le **Projet** les entités sont accessibles via des collections typées, par exemple[`Children`](../task/children) ,[`Resources`](./resources) ,[`ResourceAssignments`](./resourceassignments) , etc.

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks)
* Assemblée [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
