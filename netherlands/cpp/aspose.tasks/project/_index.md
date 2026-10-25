---
title: "Aspose::Tasks::Project klasse"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks voor C++"
description: "Stelt een project voor."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/project/
---

## Project class

Stelt een project voor.

De Project is een centrale klasse in de Aspose.Tasks-bibliotheek.

U kunt Project gebruiken om een van de ondersteunde projectmanagementformaten te lezen: MPP, MPT, MPX, XML.

Om een bestaand document in een van de ondersteunde formaten te laden, geeft u een bestandsnaam of een stream door aan een van de Project‑constructors. Om een leeg project te maken, roept u de parameterloze constructor aan.

Gebruik een van de overloads van de Save‑methode om het project op te slaan in een van de **Aspose::Tasks::Saving::SaveFileFormat**-formaten: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Vaste lay-out: PDF; Afbeeldingen: JPEG, PNG, BMP, TIFF, SVG; Tekst: TXT; Overige: HTML.

Het Project slaat projectbrede informatie op, zoals **Aspose::Tasks::Project::Views**, **Aspose::Tasks::Project::BuiltInProps**, **Aspose::Tasks::Project::CustomProps** en **Aspose::Tasks::Project::ExtendedAttributes**. De meeste van deze objecten zijn toegankelijk via de overeenkomstige eigenschappen van de Project‑klasse.

Het Project is een root‑entity die toegangspunten bevat om andere project‑entity's te manipuleren, zoals **Aspose::Tasks::Task**, **Aspose::Tasks::Resource**, **Aspose::Tasks::ResourceAssignment**, **Aspose::Tasks::ExtendedAttribute** en **Aspose::Tasks::Calendar**.

De Project‑entity's kunnen worden benaderd via getypeerde collecties, bijvoorbeeld **Aspose::Tasks::Task::Children**, **Aspose::Tasks::Project::Resources**, **Aspose::Tasks::Project::ResourceAssignments**, enzovoort.

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Project (13 overloads)](./project/) | Initialiseert een nieuwe instantie van de Project‑klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Kopieert de hoofdgegevens en eigenschappen van het project naar een ander project. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Doorloopt recursief alle taken van het project, inclusief de root‑taak. |
| [Get](./get/) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [get_ActualsInSync](./get_actualsinsync/) | Haalt een waarde op die aangeeft of ActualsInSync is ingesteld of niet. |
| [get_AdminProject](./get_adminproject/) | Haalt een waarde op die aangeeft of AdminProject is ingesteld of niet. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Haalt een waarde op die aangeeft of AreEditableActualCosts is ingesteld of niet. |
| [get_Author](./get_author/) | Haalt de waarde van Author op. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Haalt een waarde op die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Haalt op of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk van de toewijzing en de tarieven van de resource. |
| [get_Autolink](./get_autolink/) | Haalt een waarde op die aangeeft of Autolink is ingesteld of niet. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Haalt de waarde van BaselineForEarnedValue op. |
| [get_BuiltInProps](./get_builtinprops/) | Haalt de collectie met ingebouwde eigenschappen van het project op. |
| [get_CalculationMode](./get_calculationmode/) | Haalt de berekeningsmodus van een project op. Kan een van de waarden van de CalculationMode‑enumeratie zijn. |
| [get_Calendar](./get_calendar/) | Haalt een waarde op van Calendar. |
| [get_Calendars](./get_calendars/) | Haalt het CalendarCollection-object van deze Project‑instantie op. |
| [get_Category](./get_category/) | Haalt de waarde van Category op. |
| [get_Comments](./get_comments/) | Haalt de waarde van Comments op. |
| [get_Company](./get_company/) | Haalt de waarde van Company op. |
| [get_CreationDate](./get_creationdate/) | Haalt de waarde van CreationDate op. |
| [get_CriticalPath](./get_criticalpath/) | Haalt een collectie op die een lijst bevat van kritieke taken die het kritieke pad van dit project vormen. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Haalt een waarde op van CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Haalt een waarde op van CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Haalt een waarde op van CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Haalt een waarde op van CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Haalt een waarde op van CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Haalt een waarde op van CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Haalt een waarde op van CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Haalt de collectie van aangepaste projecteigenschappen op. |
| [get_DateFormat](./get_dateformat/) | Haalt een waarde op van DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Haalt een waarde op van DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Haalt een waarde op van DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Haalt een waarde op van DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Haalt een waarde op van DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Haalt een waarde op van DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Haalt een waarde op van DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Haalt een waarde op van DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Haalt een waarde op van DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Haalt de standaardweergave van het project op. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Haalt de instantie van de WeekDayCollection class op die een collectie van de standaard weekwerkdagen en werktijden van het project vertegenwoordigt. |
| [get_DisplayOptions](./get_displayoptions/) | Haalt een instantie van de ProjectDisplayOptions class op. |
| [get_DurationFormat](./get_durationformat/) | Haalt een waarde op van DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Haalt een waarde op van EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Haalt het ExtendedAttributeDefinitionCollection-object op. De collectie van definities van uitgebreide attributen (aangepaste velden) die aan een project zijn gekoppeld. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Haalt een waarde op van ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Haalt een waarde op van FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Haalt een waarde op die aangeeft of FiscalYearStart is ingesteld of niet. |
| [get_FyStartDate](./get_fystartdate/) | Haalt een waarde op van FyStartDate. |
| [get_Guid](./get_guid/) | Haalt een waarde van Guid op. |
| [get_HonorConstraints](./get_honorconstraints/) | Haalt een waarde op die aangeeft of HonorConstraints is ingesteld of niet. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Haalt een waarde op van HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Haalt een waarde op die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Haalt een waarde op die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet. |
| [get_Keywords](./get_keywords/) | Haalt een waarde op van Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Haalt een waarde op van LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Haalt een waarde op van LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Haalt een waarde op van LastSaved. |
| [get_Manager](./get_manager/) | Haalt een waarde op van Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Haalt een waarde op die aangeeft of MicrosoftProjectServerURL is ingesteld of niet. |
| [get_MinutesPerDay](./get_minutesperday/) | Haalt een waarde op van MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Haalt een waarde op van MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Haalt een waarde op die aangeeft of MoveCompletedEndsBack is ingesteld of niet. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Haalt een waarde op die aangeeft of MoveCompletedEndsForward is ingesteld of niet. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Haalt een waarde op die aangeeft of MoveRemainingStartsBack is ingesteld of niet. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Haalt een waarde op die aangeeft of MoveRemainingStartsForward is ingesteld of niet. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Haalt een waarde op die aangeeft of MultipleCriticalPaths is ingesteld of niet. |
| [get_Name](./get_name/) | Haalt een waarde van Name op. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Haalt een waarde op die aangeeft of NewTasksAreManual is ingesteld of niet. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Haalt een waarde op die aangeeft of NewTasksEffortDriven is ingesteld of niet. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Haalt een waarde op die aangeeft of NewTasksEstimated is ingesteld of niet. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Haalt een waarde op van NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Haalt een collectie op die de instanties van de OleObject-klasse bevat die gekoppeld of ingesloten zijn in dit projectbestand. |
| [get_OutlineCodes](./get_outlinecodes/) | Haalt OutlineCodeDefinitionCollection-object op. De collectie van outline code-definities die aan een project zijn gekoppeld. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Haalt een object op dat Primavera‑specifieke eigenschappen voor een project bevat, gelezen uit een Primavera‑bestand. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Haalt een waarde op die aangeeft of ProjectExternallyEdited is ingesteld of niet. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Haalt een waarde op die aangeeft of RemoveFileProperties is ingesteld of niet. |
| [get_ResourceAssignments](./get_resourceassignments/) | Haalt het ResourceAssignmentCollection‑object op. |
| [get_ResourceFilters](./get_resourcefilters/) | Haalt alle resource‑gebaseerde filterdefinities op. ResourceFilters is een verzameling van Filter‑objecten. |
| [get_ResourceGroups](./get_resourcegroups/) | Haalt alle resource‑gebaseerde groepsdefinities op. ResourceGroups is een verzameling van Group‑objecten. |
| [get_Resources](./get_resources/) | Haalt het ResourceCollection‑object op. |
| [get_Revision](./get_revision/) | Haalt een waarde van Revision op. |
| [get_RootTask](./get_roottask/) | Haalt de wortel van de boom van taken op. |
| [get_SaveVersion](./get_saveversion/) | Haalt een waarde van SaveVersion op. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Haalt een waarde op die aangeeft of ScheduleFromStart is ingesteld of niet. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Haalt een waarde op die aangeeft of ShowProjectSummaryTask is ingesteld of niet. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Haalt een waarde op die aangeeft of SplitsInProgressTasks is ingesteld of niet. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Haalt een waarde op die aangeeft of SpreadActualCost is ingesteld of niet. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Haalt een waarde op die aangeeft of SpreadPercentComplete is ingesteld of niet. |
| [get_StartDate](./get_startdate/) | Haalt een waarde van StartDate op. |
| [get_StatusDate](./get_statusdate/) | Haalt een waarde van StatusDate op. |
| [get_Subject](./get_subject/) | Haalt een waarde van Subject op. |
| [get_Tables](./get_tables/) | Haalt een lijst met Table‑objecten op. |
| [get_TaskFilters](./get_taskfilters/) | Haalt alle taak‑gebaseerde filterdefinities op. TaskFilters is een verzameling van Filter‑objecten. |
| [get_TaskGroups](./get_taskgroups/) | Haalt alle taak‑gebaseerde groepsdefinities op. TaskGroups is een verzameling van Group‑objecten. |
| [get_TaskLinks](./get_tasklinks/) | Haalt het TaskLinkCollection‑object op. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Haalt een waarde op die aangeeft of TaskUpdatesResource is ingesteld of niet. |
| [get_Template](./get_template/) | Haalt een waarde van Template op. |
| [get_TimescaleFinish](./get_timescalefinish/) | Haalt een waarde van TimescaleFinish op. |
| [get_TimescaleStart](./get_timescalestart/) | Haalt een waarde van TimescaleStart op. |
| [get_Title](./get_title/) | Haalt een waarde van Title op. |
| [get_Uid](./get_uid/) | Haalt een waarde van Uid op. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Haalt een waarde op die aangeeft of UpdateManuallyScheduledTasksWhenEditingLinks is ingesteld of niet. |
| [get_VbaProject](./get_vbaproject/) | Haalt een instantie van de VbaProject-klasse op. |
| [get_Views](./get_views/) | Haalt een lijst met View-objecten op. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Haalt de WBS Code-definitie voor het project op. |
| [get_WeekStartDay](./get_weekstartday/) | Haalt een waarde van WeekStartDay op. |
| [get_WorkFormat](./get_workformat/) | Haalt een waarde van WorkFormat op. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Retourneert de baseline-opslagtijd. |
| [GetDuration (3 overloads)](./getduration/) | Haalt een Duration-object op met het opgegeven aantal eenheden en het standaardduurformaat dat is gedefinieerd in de projectinstellingen Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard Timescale (Days). |
| [GetPredecessors](./getpredecessors/) | Retourneert een collectie van taaklinks die voorgangers zijn van de opgegeven taak. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Haalt projectbestandsinformatie op uit de stream. |
| [GetWork](./getwork/) | Haalt een Duration-object op met de opgegeven double-waarde en het standaard werkformaat. |
| [Recalculate (2 overloads)](./recalculate/) | Plant alle projecttaak‑ID's, outline-niveaus, start-/einddatums opnieuw in, stelt vroege/late datums in, berekent speling, werk- en kostvelden. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Herberekent Id, Start en Finish van resources. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Herberekent Start en Finish van resources. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Verwijdert ongeldige resource‑toewijzingen uit de lijst met projectresource‑toewijzingen. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Hernummer WBS-code van alle taken. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Plant onvoltooide projectwerk opnieuw in om te starten na een opgegeven datum. |
| [Save (5 overloads)](./save/) | Slaat het project op in een stream met de opgegeven opslagopties. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Slaat het project op als een sjabloon in een opgegeven stream. |
| [SaveReport (4 overloads)](./savereport/) | Slaat het projectoverzichtsrapport op in de stream. |
| [SelectAllChildTasks](./selectallchildtasks/) | Verzamelt recursief alle sub‑taken van de hoofdtaak. |
| [Set (2 overloads)](./set/) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [set_ActualsInSync](./set_actualsinsync/) | Stelt een waarde in die aangeeft of ActualsInSync is ingesteld of niet. |
| [set_AdminProject](./set_adminproject/) | Stelt een waarde in die aangeeft of AdminProject is ingesteld of niet. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Stelt een waarde in die aangeeft of AreEditableActualCosts is ingesteld of niet. |
| [set_Author](./set_author/) | Stelt een waarde in voor Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Stelt een waarde in die aangeeft of AutoAddNewResourcesAndTasks is ingesteld of niet. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Stelt in of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk van de toewijzing en de tarieven van de resource. |
| [set_Autolink](./set_autolink/) | Stelt een waarde in die aangeeft of Autolink is ingesteld of niet. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Stelt een waarde in voor BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Stelt de berekeningsmodus van een project in. Kan een van de waarden van de enumeratie CalculationMode zijn. |
| [set_Calendar](./set_calendar/) | Stelt een waarde in voor Calendar. |
| [set_Category](./set_category/) | Stelt een waarde in voor Category. |
| [set_Comments](./set_comments/) | Stelt een waarde in voor Comments. |
| [set_Company](./set_company/) | Stelt een waarde in voor Company. |
| [set_CreationDate](./set_creationdate/) | Stelt een waarde in voor CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Stelt een waarde in voor CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Stelt een waarde in voor CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Stelt een waarde in voor CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Stelt een waarde in voor CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Stelt een waarde in voor CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Stelt een waarde in voor CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Stelt een waarde in voor CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Stelt een waarde in voor DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Stelt een waarde in voor DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Stelt een waarde in voor DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Stelt een waarde in voor DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Stelt een waarde in voor DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Stelt een waarde in voor DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Stelt een waarde in voor DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Stelt een waarde in voor DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Stelt een waarde in voor DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Stelt de standaardweergave van het project in. |
| [set_DurationFormat](./set_durationformat/) | Stelt een waarde in voor DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Stelt een waarde in voor EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Stelt een waarde in voor ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Stelt een waarde in voor FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Stelt een waarde in die aangeeft of FiscalYearStart is ingesteld of niet. |
| [set_FyStartDate](./set_fystartdate/) | Stelt een waarde in voor FyStartDate. |
| [set_Guid](./set_guid/) | Stelt een waarde in voor Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Stelt een waarde in die aangeeft of HonorConstraints is ingesteld of niet. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Stelt een waarde in voor HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Stelt een waarde in die aangeeft of InsertedProjectsLikeSummary is ingesteld of niet. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Stelt een waarde in die aangeeft of KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is ingesteld of niet. |
| [set_Keywords](./set_keywords/) | Stelt een waarde in voor Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Stelt een waarde in voor LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Stelt een waarde in voor LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Stelt een waarde in voor LastSaved. |
| [set_Manager](./set_manager/) | Stelt een waarde in voor Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Stelt een waarde in die aangeeft of MicrosoftProjectServerURL is ingesteld of niet. |
| [set_MinutesPerDay](./set_minutesperday/) | Stelt een waarde in voor MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Stelt een waarde in voor MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Stelt een waarde in die aangeeft of MoveCompletedEndsBack is ingesteld of niet. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Stelt een waarde in die aangeeft of MoveCompletedEndsForward is ingesteld of niet. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Stelt een waarde in die aangeeft of MoveRemainingStartsBack is ingesteld of niet. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Stelt een waarde in die aangeeft of MoveRemainingStartsForward is ingesteld of niet. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Stelt een waarde in die aangeeft of MultipleCriticalPaths is ingesteld of niet. |
| [set_Name](./set_name/) | Stelt een waarde in van Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Stelt een waarde in die aangeeft of NewTasksAreManual is ingesteld of niet. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Stelt een waarde in die aangeeft of NewTasksEffortDriven is ingesteld of niet. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Stelt een waarde in die aangeeft of NewTasksEstimated is ingesteld of niet. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Stelt een waarde in voor NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Stelt een waarde in die aangeeft of ProjectExternallyEdited is ingesteld of niet. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Stelt een waarde in die aangeeft of RemoveFileProperties is ingesteld of niet. |
| [set_Revision](./set_revision/) | Stelt een waarde in voor Revision. |
| [set_SaveVersion](./set_saveversion/) | Stelt een waarde in voor SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Stelt een waarde in die aangeeft of ScheduleFromStart is ingesteld of niet. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Stelt een waarde in die aangeeft of ShowProjectSummaryTask is ingesteld of niet. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Stelt een waarde in die aangeeft of SplitsInProgressTasks is ingesteld of niet. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Stelt een waarde in die aangeeft of SpreadActualCost is ingesteld of niet. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Stelt een waarde in die aangeeft of SpreadPercentComplete is ingesteld of niet. |
| [set_StartDate](./set_startdate/) | Stelt een waarde in voor StartDate. |
| [set_StatusDate](./set_statusdate/) | Stelt een waarde in voor StatusDate. |
| [set_Subject](./set_subject/) | Stelt een waarde in voor Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Stelt een waarde in die aangeeft of TaskUpdatesResource is ingesteld of niet. |
| [set_Template](./set_template/) | Stelt een waarde in voor Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Stelt een waarde in voor TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Stelt een waarde in voor TimescaleStart. |
| [set_Title](./set_title/) | Stelt een waarde in voor Title. |
| [set_Uid](./set_uid/) | Stelt een waarde in van Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Stelt een waarde in die aangeeft of UpdateManuallyScheduledTasksWhenEditingLinks is ingesteld of niet. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Stelt de WBS Code-definitie in voor het project. |
| [set_WeekStartDay](./set_weekstartday/) | Stelt een waarde in voor WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Stelt een waarde in voor WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Slaat basislijnvelden op naar de opgegeven basislijn voor het gehele project. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Stelt de tijd voor het opslaan van de basislijn in. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Werk alle werkzaamheden bij als voltooid tot een opgegeven datum voor het gehele project. |

