---
title: "Classe Aspose::Tasks::Project"
linktitle: "Projet"
articleTitle: "Projet"
second_title: "Aspose.Tasks pour C++"
description: "Représente un projet."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/project/
---

## Project class

Représente un projet.

Le Projet est une classe centrale dans la bibliothèque Aspose.Tasks.

On peut utiliser Project pour lire l'un des formats de gestion de projet pris en charge : MPP, MPT, MPX, XML.

Pour charger un document existant dans l'un des formats pris en charge, transmettez un nom de fichier ou un flux à l'un des constructeurs de Project. Pour créer un projet vierge, appelez le constructeur sans paramètres.

Utilisez l'une des surcharges de la méthode Save pour enregistrer le projet dans l'un des formats Aspose::Tasks::Saving::SaveFileFormat : Primavera : P6 XML, PM XER ; Microsoft Excel : XLSX, XML ; Mise en page fixe : PDF ; Images : JPEG, PNG, BMP, TIFF, SVG ; Texte : TXT ; Autres : HTML.

Le Project stocke des informations à l'échelle du projet telles que Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps et Aspose::Tasks::Project::ExtendedAttributes. La plupart de ces objets sont accessibles via les propriétés correspondantes de la classe Project.

Le Project est une entité racine qui contient des points d'entrée pour manipuler d'autres entités du projet, telles que Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute et Aspose::Tasks::Calendar.

Les entités du Project peuvent être accessibles via des collections typées, par exemple Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments, etc.

## Constructeurs

| Nom | Description |
| --- | --- |
| [Project (13 overloads)](./project/) | Initialise une nouvelle instance de la classe Project. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Copie les données principales et les propriétés du projet vers un autre projet. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Énumère récursivement toutes les tâches du projet, y compris la tâche racine. |
| [Get](./get/) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [get_ActualsInSync](./get_actualsinsync/) | Obtient une valeur indiquant si ActualsInSync est défini ou non. |
| [get_AdminProject](./get_adminproject/) | Obtient une valeur indiquant si AdminProject est défini ou non. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Obtient une valeur indiquant si AreEditableActualCosts est défini ou non. |
| [get_Author](./get_author/) | Obtient la valeur de Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Obtient une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Obtient si le coût de l'affectation et le coût restant doivent être calculés automatiquement à l'aide du travail de l'affectation et des taux des ressources. |
| [get_Autolink](./get_autolink/) | Obtient une valeur indiquant si Autolink est défini ou non. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Obtient la valeur de BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Obtient la collection des propriétés intégrées du projet. |
| [get_CalculationMode](./get_calculationmode/) | Obtient le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération CalculationMode. |
| [get_Calendar](./get_calendar/) | Obtient une valeur de Calendar. |
| [get_Calendars](./get_calendars/) | Obtient l'objet CalendarCollection de cette instance de Project. |
| [get_Category](./get_category/) | Obtient la valeur de Category. |
| [get_Comments](./get_comments/) | Obtient la valeur de Comments. |
| [get_Company](./get_company/) | Obtient la valeur de Company. |
| [get_CreationDate](./get_creationdate/) | Obtient la valeur de CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Obtient une collection qui contient une liste de tâches Critical qui composent le Chemin critique de ce projet. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Obtient une valeur de CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Obtient une valeur de CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Obtient une valeur de CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Obtient une valeur de CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Obtient une valeur de CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Obtient une valeur de CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Obtient une valeur de CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Obtient la collection des propriétés personnalisées du projet. |
| [get_DateFormat](./get_dateformat/) | Obtient une valeur de DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Obtient une valeur de DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Obtient une valeur de DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Obtient une valeur de DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Obtient une valeur de DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Obtient une valeur de DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Obtient une valeur de DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Obtient une valeur de DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Obtient une valeur de DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Obtient la vue par défaut du projet. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Obtient l'instance de la classe WeekDayCollection qui représente une collection des jours ouvrés et des heures de travail par défaut du projet. |
| [get_DisplayOptions](./get_displayoptions/) | Obtient une instance de la classe ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Obtient une valeur de DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Obtient une valeur de EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Obtient l'objet ExtendedAttributeDefinitionCollection. La collection des définitions d'attributs étendus (champs personnalisés) associées à un projet. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Obtient une valeur de ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Obtient une valeur de FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Obtient une valeur indiquant si FiscalYearStart est défini ou non. |
| [get_FyStartDate](./get_fystartdate/) | Obtient une valeur de FyStartDate. |
| [get_Guid](./get_guid/) | Obtient une valeur de Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Obtient une valeur indiquant si HonorConstraints est défini ou non. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Obtient une valeur de HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Obtient une valeur indiquant si InsertedProjectsLikeSummary est défini ou non. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Obtient une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non. |
| [get_Keywords](./get_keywords/) | Obtient une valeur de Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Obtient une valeur de LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Obtient une valeur de LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Obtient une valeur de LastSaved. |
| [get_Manager](./get_manager/) | Obtient une valeur de Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Obtient une valeur indiquant si MicrosoftProjectServerURL est défini ou non. |
| [get_MinutesPerDay](./get_minutesperday/) | Obtient une valeur de MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Obtient une valeur de MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Obtient une valeur indiquant si MoveCompletedEndsBack est défini ou non. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Obtient une valeur indiquant si MoveCompletedEndsForward est défini ou non. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Obtient une valeur indiquant si MoveRemainingStartsBack est défini ou non. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Obtient une valeur indiquant si MoveRemainingStartsForward est défini ou non. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Obtient une valeur indiquant si MultipleCriticalPaths est défini ou non. |
| [get_Name](./get_name/) | Obtient une valeur de Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Obtient une valeur indiquant si NewTasksAreManual est défini ou non. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Obtient une valeur indiquant si NewTasksEffortDriven est défini ou non. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Obtient une valeur indiquant si NewTasksEstimated est défini ou non. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Obtient une valeur de NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Obtient une collection contenant les instances de la classe OleObject qui sont liées ou incorporées à ce fichier de projet. |
| [get_OutlineCodes](./get_outlinecodes/) | Obtient l'objet OutlineCodeDefinitionCollection. La collection des définitions de codes de plan associées à un projet. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Obtient un objet contenant des propriétés spécifiques à Primavera pour un projet lu à partir d'un fichier Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Obtient une valeur indiquant si ProjectExternallyEdited est défini ou non. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Obtient une valeur indiquant si RemoveFileProperties est défini ou non. |
| [get_ResourceAssignments](./get_resourceassignments/) | Obtient l'objet ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Obtient toutes les définitions de filtres basées sur les ressources. ResourceFilters est une collection d'objets Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Obtient toutes les définitions de groupes basées sur les ressources. ResourceGroups est une collection d'objets Group. |
| [get_Resources](./get_resources/) | Obtient l'objet ResourceCollection. |
| [get_Revision](./get_revision/) | Obtient une valeur de Revision. |
| [get_RootTask](./get_roottask/) | Obtient la racine de l'arbre des tâches. |
| [get_SaveVersion](./get_saveversion/) | Obtient une valeur de SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Obtient une valeur indiquant si ScheduleFromStart est défini ou non. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Obtient une valeur indiquant si ShowProjectSummaryTask est défini ou non. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Obtient une valeur indiquant si SplitsInProgressTasks est défini ou non. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Obtient une valeur indiquant si SpreadActualCost est défini ou non. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Obtient une valeur indiquant si SpreadPercentComplete est défini ou non. |
| [get_StartDate](./get_startdate/) | Obtient une valeur de StartDate. |
| [get_StatusDate](./get_statusdate/) | Obtient une valeur de StatusDate. |
| [get_Subject](./get_subject/) | Obtient une valeur de Subject. |
| [get_Tables](./get_tables/) | Obtient une liste d'objets Table. |
| [get_TaskFilters](./get_taskfilters/) | Obtient toutes les définitions de filtres basées sur les tâches. TaskFilters est une collection d'objets Filter. |
| [get_TaskGroups](./get_taskgroups/) | Obtient toutes les définitions de groupes basées sur les tâches. TaskGroups est une collection d'objets Group. |
| [get_TaskLinks](./get_tasklinks/) | Obtient l'objet TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Obtient une valeur indiquant si TaskUpdatesResource est défini ou non. |
| [get_Template](./get_template/) | Obtient une valeur de Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Obtient une valeur de TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Obtient une valeur de TimescaleStart. |
| [get_Title](./get_title/) | Obtient une valeur de Title. |
| [get_Uid](./get_uid/) | Obtient une valeur de Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Obtient une valeur indiquant si UpdateManuallyScheduledTasksWhenEditingLinks est défini ou non. |
| [get_VbaProject](./get_vbaproject/) | Obtient une instance de la classe VbaProject. |
| [get_Views](./get_views/) | Obtient une liste d'objets View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Obtient la définition du code WBS pour le projet. |
| [get_WeekStartDay](./get_weekstartday/) | Obtient une valeur de WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Obtient une valeur de WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Renvoie le temps d'enregistrement de la ligne de base. |
| [GetDuration (3 overloads)](./getduration/) | Obtient un objet Duration avec le nombre d'unités spécifié et le format de durée par défaut qui est défini dans les paramètres du projet Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Renvoie le nombre de pages du projet à rendre en utilisant l'échelle de temps par défaut (Jours). |
| [GetPredecessors](./getpredecessors/) | Renvoie une collection de liens de tâche qui sont les prédécesseurs de la tâche spécifiée. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Obtient les informations du fichier de projet depuis le flux. |
| [GetWork](./getwork/) | Obtient un objet Duration avec la valeur double spécifiée et le format de travail par défaut. |
| [Recalculate (2 overloads)](./recalculate/) | Replanifie tous les identifiants des tâches du projet, les niveaux de plan, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Recalcule l'Id, le Début et la Fin des ressources. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Recalcule le Début et la Fin des ressources. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Élimine les affectations de ressources invalides de la liste des affectations de ressources du projet. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Renumérote le code WBS de toutes les tâches. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Replanifie le travail du projet non terminé pour commencer après une date spécifiée. |
| [Save (5 overloads)](./save/) | Enregistre le projet dans un flux en utilisant les options d'enregistrement spécifiées. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Enregistre le projet en tant que modèle dans un flux spécifié. |
| [SaveReport (4 overloads)](./savereport/) | Enregistre le rapport d'aperçu du projet dans le flux. |
| [SelectAllChildTasks](./selectallchildtasks/) | Collecte récursivement toutes les sous‑tâches de la tâche racine. |
| [Set (2 overloads)](./set/) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [set_ActualsInSync](./set_actualsinsync/) | Définit une valeur indiquant si ActualsInSync est défini ou non. |
| [set_AdminProject](./set_adminproject/) | Définit une valeur indiquant si AdminProject est défini ou non. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Définit une valeur indiquant si AreEditableActualCosts est défini ou non. |
| [set_Author](./set_author/) | Définit une valeur pour Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Définit une valeur indiquant si AutoAddNewResourcesAndTasks est défini ou non. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Définit si le coût de l'affectation et le coût restant doivent être calculés automatiquement en utilisant le travail de l'affectation et les taux des ressources. |
| [set_Autolink](./set_autolink/) | Définit une valeur indiquant si Autolink est défini ou non. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Définit une valeur pour BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Définit le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération CalculationMode. |
| [set_Calendar](./set_calendar/) | Définit une valeur de Calendar. |
| [set_Category](./set_category/) | Définit une valeur pour Category. |
| [set_Comments](./set_comments/) | Définit une valeur pour Comments. |
| [set_Company](./set_company/) | Définit une valeur pour Company. |
| [set_CreationDate](./set_creationdate/) | Définit une valeur pour CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Définit une valeur pour CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Définit une valeur pour CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Définit une valeur pour CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Définit une valeur pour CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Définit une valeur pour CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Définit une valeur pour CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Définit une valeur pour CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Définit une valeur pour DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Définit une valeur pour DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Définit une valeur pour DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Définit une valeur pour DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Définit une valeur pour DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Définit une valeur pour DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Définit une valeur de DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Définit une valeur de DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Définit une valeur de DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Définit la vue par défaut du projet. |
| [set_DurationFormat](./set_durationformat/) | Définit une valeur de DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Définit une valeur de EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Définit une valeur de ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Définit une valeur de FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Définit une valeur indiquant si FiscalYearStart est défini ou non. |
| [set_FyStartDate](./set_fystartdate/) | Définit une valeur de FyStartDate. |
| [set_Guid](./set_guid/) | Définit une valeur de Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Définit une valeur indiquant si HonorConstraints est défini ou non. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Définit une valeur de HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Définit une valeur indiquant si InsertedProjectsLikeSummary est défini ou non. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Définit une valeur indiquant si KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled est défini ou non. |
| [set_Keywords](./set_keywords/) | Définit une valeur de Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Définit une valeur de LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Définit une valeur de LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Définit une valeur de LastSaved. |
| [set_Manager](./set_manager/) | Définit une valeur de Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Définit une valeur indiquant si MicrosoftProjectServerURL est défini ou non. |
| [set_MinutesPerDay](./set_minutesperday/) | Définit une valeur de MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Définit une valeur de MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Définit une valeur indiquant si MoveCompletedEndsBack est défini ou non. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Définit une valeur indiquant si MoveCompletedEndsForward est défini ou non. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Définit une valeur indiquant si MoveRemainingStartsBack est défini ou non. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Définit une valeur indiquant si MoveRemainingStartsForward est défini ou non. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Définit une valeur indiquant si MultipleCriticalPaths est défini ou non. |
| [set_Name](./set_name/) | Définit une valeur de Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Définit une valeur indiquant si NewTasksAreManual est défini ou non. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Définit une valeur indiquant si NewTasksEffortDriven est défini ou non. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Définit une valeur indiquant si NewTasksEstimated est défini ou non. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Définit une valeur de NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Définit une valeur indiquant si ProjectExternallyEdited est défini ou non. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Définit une valeur indiquant si RemoveFileProperties est défini ou non. |
| [set_Revision](./set_revision/) | Définit une valeur de Revision. |
| [set_SaveVersion](./set_saveversion/) | Définit une valeur de SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Définit une valeur indiquant si ScheduleFromStart est défini ou non. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Définit une valeur indiquant si ShowProjectSummaryTask est défini ou non. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Définit une valeur indiquant si SplitsInProgressTasks est défini ou non. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Définit une valeur indiquant si SpreadActualCost est défini ou non. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Définit une valeur indiquant si SpreadPercentComplete est défini ou non. |
| [set_StartDate](./set_startdate/) | Définit une valeur de StartDate. |
| [set_StatusDate](./set_statusdate/) | Définit une valeur de StatusDate. |
| [set_Subject](./set_subject/) | Définit une valeur de Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Définit une valeur indiquant si TaskUpdatesResource est défini ou non. |
| [set_Template](./set_template/) | Définit une valeur de Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Définit une valeur de TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Définit une valeur de TimescaleStart. |
| [set_Title](./set_title/) | Définit une valeur de Title. |
| [set_Uid](./set_uid/) | Définit une valeur de Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Définit une valeur indiquant si UpdateManuallyScheduledTasksWhenEditingLinks est défini ou non. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Définit la définition du code WBS pour le projet. |
| [set_WeekStartDay](./set_weekstartday/) | Définit une valeur de WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Définit une valeur de WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Enregistre les champs de référence dans la référence spécifiée pour l'ensemble du projet. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Définit l'heure d'enregistrement de la référence. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour l'ensemble du projet. |

