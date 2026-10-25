---
title: "Aspose::Tasks::Project Klasse"
linktitle: "Projekt"
articleTitle: "Projekt"
second_title: "Aspose.Tasks für C++"
description: "Stellt ein Projekt dar."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/project/
---

## Project class

Stellt ein Projekt dar.

Das Projekt ist eine zentrale Klasse in der Bibliothek Aspose.Tasks.

Man kann Project verwenden, um eines der unterstützten Projektmanagement‑Formate zu lesen: MPP, MPT, MPX, XML.

Um ein vorhandenes Dokument in einem der unterstützten Formate zu laden, übergeben Sie einen Dateinamen oder einen Stream an einen der Project‑Konstruktoren. Um ein leeres Projekt zu erstellen, rufen Sie den parameterlosen Konstruktor auf.

Verwenden Sie eine der Überladungen der Save‑Methode, um das Projekt in einem der Aspose::Tasks::Saving::SaveFileFormat‑Formate zu speichern: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Festes Layout: PDF; Bilder: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Sonstige: HTML.

Das Project speichert projektweite Informationen wie Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps und Aspose::Tasks::Project::ExtendedAttributes. Die meisten dieser Objekte sind über die entsprechenden Eigenschaften der Project‑Klasse zugänglich.

Das Project ist eine Root‑Entität, die Einstiegspunkte enthält, um andere Projektelemente zu manipulieren, wie Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute und Aspose::Tasks::Calendar.

Auf die Project‑Entitäten kann über typisierte Sammlungen zugegriffen werden, zum Beispiel Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments usw.

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Project (13 overloads)](./project/) | Initialisiert eine neue Instanz der Project‑Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Kopiert die Hauptdaten und Eigenschaften des Projekts in ein anderes Projekt. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Enumeriert rekursiv alle Aufgaben des Projekts einschließlich der Root‑Aufgabe. |
| [Get](./get/) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [get_ActualsInSync](./get_actualsinsync/) | Gibt einen Wert zurück, der angibt, ob ActualsInSync gesetzt ist oder nicht. |
| [get_AdminProject](./get_adminproject/) | Gibt einen Wert zurück, der angibt, ob AdminProject gesetzt ist oder nicht. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Gibt einen Wert zurück, der angibt, ob AreEditableActualCosts gesetzt ist oder nicht. |
| [get_Author](./get_author/) | Gibt den Wert von Author zurück. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Gibt einen Wert zurück, der angibt, ob AutoAddNewResourcesAndTasks gesetzt ist oder nicht. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Gibt an, ob die Zuweisungskosten und Restkosten automatisch anhand der Arbeitszeit der Zuweisung und der Ressourcensätze berechnet werden sollen. |
| [get_Autolink](./get_autolink/) | Gibt einen Wert zurück, der angibt, ob Autolink gesetzt ist oder nicht. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Gibt den Wert von BaselineForEarnedValue zurück. |
| [get_BuiltInProps](./get_builtinprops/) | Gibt die Sammlung der integrierten Projekteigenschaften zurück. |
| [get_CalculationMode](./get_calculationmode/) | Gibt den Berechnungsmodus eines Projekts zurück. Kann einer der Werte der Aufzählung CalculationMode sein. |
| [get_Calendar](./get_calendar/) | Gibt einen Wert von Calendar zurück. |
| [get_Calendars](./get_calendars/) | Gibt das CalendarCollection‑Objekt dieser Project‑Instanz zurück. |
| [get_Category](./get_category/) | Gibt den Wert von Category zurück. |
| [get_Comments](./get_comments/) | Gibt den Wert von Comments zurück. |
| [get_Company](./get_company/) | Gibt den Wert von Company zurück. |
| [get_CreationDate](./get_creationdate/) | Gibt den Wert von CreationDate zurück. |
| [get_CriticalPath](./get_criticalpath/) | Gibt eine Sammlung zurück, die eine Liste kritischer Aufgaben enthält, die den kritischen Pfad dieses Projekts bilden. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Liefert einen Wert von CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Liefert einen Wert von CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Liefert einen Wert von CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Liefert einen Wert von CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Liefert einen Wert von CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Liefert einen Wert von CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Liefert einen Wert von CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Liefert die benutzerdefinierte Eigenschaften-Sammlung des Projekts. |
| [get_DateFormat](./get_dateformat/) | Liefert einen Wert von DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Liefert einen Wert von DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Liefert einen Wert von DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Liefert einen Wert von DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Liefert einen Wert von DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Liefert einen Wert von DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Liefert einen Wert von DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Liefert einen Wert von DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Liefert einen Wert von DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Liefert die Standardansicht des Projekts. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Liefert die Instanz der Klasse WeekDayCollection, die eine Sammlung der standardmäßigen Wochenarbeitstage und Arbeitszeiten des Projekts darstellt. |
| [get_DisplayOptions](./get_displayoptions/) | Liefert eine Instanz der Klasse ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Liefert einen Wert von DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Liefert einen Wert von EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Liefert das Objekt ExtendedAttributeDefinitionCollection. Die Sammlung der Definitionen erweiterter Attribute (benutzerdefinierter Felder), die einem Projekt zugeordnet sind. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Liefert einen Wert von ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Liefert einen Wert von FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Gibt einen Wert zurück, der angibt, ob FiscalYearStart gesetzt ist oder nicht. |
| [get_FyStartDate](./get_fystartdate/) | Gibt den Wert von FyStartDate zurück. |
| [get_Guid](./get_guid/) | Ruft den Wert von Guid ab. |
| [get_HonorConstraints](./get_honorconstraints/) | Gibt einen Wert zurück, der angibt, ob HonorConstraints gesetzt ist oder nicht. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Gibt den Wert von HyperlinkBase zurück. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Gibt einen Wert zurück, der angibt, ob InsertedProjectsLikeSummary gesetzt ist oder nicht. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Gibt einen Wert zurück, der angibt, ob KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled gesetzt ist oder nicht. |
| [get_Keywords](./get_keywords/) | Gibt den Wert von Keywords zurück. |
| [get_LastAuthor](./get_lastauthor/) | Gibt den Wert von LastAuthor zurück. |
| [get_LastPrinted](./get_lastprinted/) | Gibt den Wert von LastPrinted zurück. |
| [get_LastSaved](./get_lastsaved/) | Gibt den Wert von LastSaved zurück. |
| [get_Manager](./get_manager/) | Gibt den Wert von Manager zurück. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Gibt einen Wert zurück, der angibt, ob MicrosoftProjectServerURL gesetzt ist oder nicht. |
| [get_MinutesPerDay](./get_minutesperday/) | Gibt den Wert von MinutesPerDay zurück. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Gibt den Wert von MinutesPerWeek zurück. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsBack gesetzt ist oder nicht. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Gibt einen Wert zurück, der angibt, ob MoveCompletedEndsForward gesetzt ist oder nicht. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsBack gesetzt ist oder nicht. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Gibt einen Wert zurück, der angibt, ob MoveRemainingStartsForward gesetzt ist oder nicht. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Gibt einen Wert zurück, der angibt, ob MultipleCriticalPaths gesetzt ist oder nicht. |
| [get_Name](./get_name/) | Ruft den Wert von Name ab. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Gibt einen Wert zurück, der angibt, ob NewTasksAreManual gesetzt ist oder nicht. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Gibt einen Wert zurück, der angibt, ob NewTasksEffortDriven gesetzt ist oder nicht. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Gibt einen Wert zurück, der angibt, ob NewTasksEstimated gesetzt ist oder nicht. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Gibt den Wert von NewTaskStartDate zurück. |
| [get_OleObjects](./get_oleobjects/) | Gibt eine Sammlung zurück, die die Instanzen der Klasse OleObject enthält, die mit dieser Projektdatei verknüpft oder eingebettet sind. |
| [get_OutlineCodes](./get_outlinecodes/) | Gibt das OutlineCodeDefinitionCollection-Objekt zurück. Die Sammlung der Gliederungscode-Definitionen, die einem Projekt zugeordnet sind. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Liefert ein Objekt, das Primavera-spezifische Eigenschaften für ein Projekt enthält, das aus einer Primavera-Datei gelesen wurde. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Liefert einen Wert, der angibt, ob ProjectExternallyEdited gesetzt ist oder nicht. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Liefert einen Wert, der angibt, ob RemoveFileProperties gesetzt ist oder nicht. |
| [get_ResourceAssignments](./get_resourceassignments/) | Liefert das ResourceAssignmentCollection-Objekt. |
| [get_ResourceFilters](./get_resourcefilters/) | Liefert alle ressourcenbasierten Filterdefinitionen. ResourceFilters ist eine Sammlung von Filter-Objekten. |
| [get_ResourceGroups](./get_resourcegroups/) | Liefert alle ressourcenbasierten Gruppendefinitionen. ResourceGroups ist eine Sammlung von Group-Objekten. |
| [get_Resources](./get_resources/) | Liefert das ResourceCollection-Objekt. |
| [get_Revision](./get_revision/) | Liefert einen Wert von Revision. |
| [get_RootTask](./get_roottask/) | Liefert die Wurzel des Aufgabenbaums. |
| [get_SaveVersion](./get_saveversion/) | Liefert einen Wert von SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Liefert einen Wert, der angibt, ob ScheduleFromStart gesetzt ist oder nicht. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Liefert einen Wert, der angibt, ob ShowProjectSummaryTask gesetzt ist oder nicht. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Liefert einen Wert, der angibt, ob SplitsInProgressTasks gesetzt ist oder nicht. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Liefert einen Wert, der angibt, ob SpreadActualCost gesetzt ist oder nicht. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Liefert einen Wert, der angibt, ob SpreadPercentComplete gesetzt ist oder nicht. |
| [get_StartDate](./get_startdate/) | Liefert einen Wert von StartDate. |
| [get_StatusDate](./get_statusdate/) | Liefert einen Wert von StatusDate. |
| [get_Subject](./get_subject/) | Liefert einen Wert von Subject. |
| [get_Tables](./get_tables/) | Liefert eine Liste von Table-Objekten. |
| [get_TaskFilters](./get_taskfilters/) | Liefert alle aufgabenbasierten Filterdefinitionen. TaskFilters ist eine Sammlung von Filter-Objekten. |
| [get_TaskGroups](./get_taskgroups/) | Liefert alle aufgabenbasierten Gruppendefinitionen. TaskGroups ist eine Sammlung von Group-Objekten. |
| [get_TaskLinks](./get_tasklinks/) | Liefert das TaskLinkCollection-Objekt. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Liefert einen Wert, der angibt, ob TaskUpdatesResource gesetzt ist oder nicht. |
| [get_Template](./get_template/) | Liefert einen Wert von Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Liefert einen Wert von TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Ruft einen Wert von TimescaleStart ab. |
| [get_Title](./get_title/) | Ruft einen Wert von Title ab. |
| [get_Uid](./get_uid/) | Ruft einen Wert von Uid ab. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Ruft einen Wert ab, der angibt, ob UpdateManuallyScheduledTasksWhenEditingLinks gesetzt ist oder nicht. |
| [get_VbaProject](./get_vbaproject/) | Ruft eine Instanz der Klasse VbaProject ab. |
| [get_Views](./get_views/) | Ruft eine Liste von View-Objekten ab. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Ruft die WBS Code Definition für das Projekt ab. |
| [get_WeekStartDay](./get_weekstartday/) | Ruft einen Wert von WeekStartDay ab. |
| [get_WorkFormat](./get_workformat/) | Ruft einen Wert von WorkFormat ab. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Gibt die Basis-Speicherzeit zurück. |
| [GetDuration (3 overloads)](./getduration/) | Ruft ein Duration-Objekt mit der angegebenen Anzahl von Einheiten und dem Standard-Dauerformat ab, das in den Projekteinstellungen Prj::DurationFormat definiert ist. |
| [GetPageCount (7 overloads)](./getpagecount/) | Gibt die Seitenanzahl für das Projekt zurück, das mit der Standard Timescale (Days) gerendert wird. |
| [GetPredecessors](./getpredecessors/) | Gibt eine Sammlung von Aufgabenverknüpfungen zurück, die Vorgänger der angegebenen Aufgabe sind. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Ruft Projektdateiinformationen aus dem Stream ab. |
| [GetWork](./getwork/) | Ruft ein Duration-Objekt mit dem angegebenen Double-Wert und dem Standard-Arbeitsformat ab. |
| [Recalculate (2 overloads)](./recalculate/) | Plant alle Projektaufgaben-IDs, Gliederungsebenen, Start-/Enddaten neu, setzt Früh-/Spättermine, berechnet Puffer, Arbeits- und Kostenfelder. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Rechnet Id, Start und Ende von Ressourcen neu. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Rechnet Start und Ende von Ressourcen neu. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Eliminiert ungültige Ressourcen-Zuweisungen aus der Projektressourcenzuweisungsliste. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Nummeriert den WBS-Code aller Aufgaben neu. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Plant nicht abgeschlossene Projektarbeit so um, dass sie nach einem angegebenen Datum beginnt. |
| [Save (5 overloads)](./save/) | Speichert das Projekt in einen Stream unter Verwendung der angegebenen Speicheroptionen. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Speichert das Projekt als Vorlage in einen angegebenen Stream. |
| [SaveReport (4 overloads)](./savereport/) | Speichert den Projektübersichtsbericht in den Stream. |
| [SelectAllChildTasks](./selectallchildtasks/) | Sammelt rekursiv alle Unteraufgaben der Wurzelaufgabe. |
| [Set (2 overloads)](./set/) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [set_ActualsInSync](./set_actualsinsync/) | Setzt einen Wert, der angibt, ob ActualsInSync gesetzt ist oder nicht. |
| [set_AdminProject](./set_adminproject/) | Legt einen Wert fest, der angibt, ob AdminProject gesetzt ist oder nicht. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Legt einen Wert fest, der angibt, ob AreEditableActualCosts gesetzt ist oder nicht. |
| [set_Author](./set_author/) | Legt einen Wert für Author fest. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Legt einen Wert fest, der angibt, ob AutoAddNewResourcesAndTasks gesetzt ist oder nicht. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Legt fest, ob die Zuweisungskosten und Restkosten automatisch anhand der Arbeitszeit der Zuweisung und der Ressourcensätze berechnet werden sollen. |
| [set_Autolink](./set_autolink/) | Legt einen Wert fest, der angibt, ob Autolink gesetzt ist oder nicht. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Legt einen Wert für BaselineForEarnedValue fest. |
| [set_CalculationMode](./set_calculationmode/) | Legt den Berechnungsmodus eines Projekts fest. Kann einer der Werte der Aufzählung CalculationMode sein. |
| [set_Calendar](./set_calendar/) | Setzt einen Wert von Calendar. |
| [set_Category](./set_category/) | Legt einen Wert für Category fest. |
| [set_Comments](./set_comments/) | Legt einen Wert für Comments fest. |
| [set_Company](./set_company/) | Legt einen Wert für Company fest. |
| [set_CreationDate](./set_creationdate/) | Legt einen Wert für CreationDate fest. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Legt einen Wert für CriticalSlackLimit fest. |
| [set_CurrencyCode](./set_currencycode/) | Legt einen Wert für CurrencyCode fest. |
| [set_CurrencyDigits](./set_currencydigits/) | Legt einen Wert für CurrencyDigits fest. |
| [set_CurrencySymbol](./set_currencysymbol/) | Legt einen Wert für CurrencySymbol fest. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Legt einen Wert für CurrencySymbolPosition fest. |
| [set_CurrentDate](./set_currentdate/) | Legt einen Wert für CurrentDate fest. |
| [set_CustomDateFormat](./set_customdateformat/) | Legt einen Wert für CustomDateFormat fest. |
| [set_DateFormat](./set_dateformat/) | Legt einen Wert für DateFormat fest. |
| [set_DaysPerMonth](./set_dayspermonth/) | Legt einen Wert für DaysPerMonth fest. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Legt einen Wert für DefaultFinishTime fest. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Legt einen Wert für DefaultFixedCostAccrual fest. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Legt einen Wert für DefaultOvertimeRate fest. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Legt einen Wert für DefaultStandardRate fest. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Setzt einen Wert von DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Setzt einen Wert von DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Setzt einen Wert von DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Setzt die Standardansicht des Projekts. |
| [set_DurationFormat](./set_durationformat/) | Setzt einen Wert von DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Setzt einen Wert von EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Setzt einen Wert von ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Setzt einen Wert von FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Setzt einen Wert, der angibt, ob FiscalYearStart gesetzt ist oder nicht. |
| [set_FyStartDate](./set_fystartdate/) | Setzt einen Wert von FyStartDate. |
| [set_Guid](./set_guid/) | Setzt einen Wert von Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Setzt einen Wert, der angibt, ob HonorConstraints gesetzt ist oder nicht. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Setzt einen Wert von HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Setzt einen Wert, der angibt, ob InsertedProjectsLikeSummary gesetzt ist oder nicht. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Setzt einen Wert, der angibt, ob KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled gesetzt ist oder nicht. |
| [set_Keywords](./set_keywords/) | Setzt einen Wert von Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Setzt einen Wert von LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Setzt einen Wert von LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Setzt einen Wert von LastSaved. |
| [set_Manager](./set_manager/) | Setzt einen Wert von Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Setzt einen Wert, der angibt, ob MicrosoftProjectServerURL gesetzt ist oder nicht. |
| [set_MinutesPerDay](./set_minutesperday/) | Setzt einen Wert von MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Setzt einen Wert von MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Setzt einen Wert, der angibt, ob MoveCompletedEndsBack gesetzt ist oder nicht. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Setzt einen Wert, der angibt, ob MoveCompletedEndsForward gesetzt ist oder nicht. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Setzt einen Wert, der angibt, ob MoveRemainingStartsBack gesetzt ist oder nicht. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Legt einen Wert fest, der angibt, ob MoveRemainingStartsForward gesetzt ist oder nicht. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Legt einen Wert fest, der angibt, ob MultipleCriticalPaths gesetzt ist oder nicht. |
| [set_Name](./set_name/) | Setzt einen Wert von Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Legt einen Wert fest, der angibt, ob NewTasksAreManual gesetzt ist oder nicht. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Legt einen Wert fest, der angibt, ob NewTasksEffortDriven gesetzt ist oder nicht. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Legt einen Wert fest, der angibt, ob NewTasksEstimated gesetzt ist oder nicht. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Legt einen Wert für NewTaskStartDate fest. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Legt einen Wert fest, der angibt, ob ProjectExternallyEdited gesetzt ist oder nicht. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Legt einen Wert fest, der angibt, ob RemoveFileProperties gesetzt ist oder nicht. |
| [set_Revision](./set_revision/) | Legt einen Wert für Revision fest. |
| [set_SaveVersion](./set_saveversion/) | Legt einen Wert für SaveVersion fest. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Legt einen Wert fest, der angibt, ob ScheduleFromStart gesetzt ist oder nicht. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Legt einen Wert fest, der angibt, ob ShowProjectSummaryTask gesetzt ist oder nicht. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Legt einen Wert fest, der angibt, ob SplitsInProgressTasks gesetzt ist oder nicht. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Legt einen Wert fest, der angibt, ob SpreadActualCost gesetzt ist oder nicht. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Legt einen Wert fest, der angibt, ob SpreadPercentComplete gesetzt ist oder nicht. |
| [set_StartDate](./set_startdate/) | Legt einen Wert für StartDate fest. |
| [set_StatusDate](./set_statusdate/) | Legt einen Wert für StatusDate fest. |
| [set_Subject](./set_subject/) | Legt einen Wert für Subject fest. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Legt einen Wert fest, der angibt, ob TaskUpdatesResource gesetzt ist oder nicht. |
| [set_Template](./set_template/) | Legt einen Wert für Template fest. |
| [set_TimescaleFinish](./set_timescalefinish/) | Legt einen Wert für TimescaleFinish fest. |
| [set_TimescaleStart](./set_timescalestart/) | Legt einen Wert für TimescaleStart fest. |
| [set_Title](./set_title/) | Legt einen Wert für Title fest. |
| [set_Uid](./set_uid/) | Setzt einen Wert von Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Legt einen Wert fest, der angibt, ob UpdateManuallyScheduledTasksWhenEditingLinks gesetzt ist oder nicht. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Legt die WBS-Code-Definition für das Projekt fest. |
| [set_WeekStartDay](./set_weekstartday/) | Setzt einen Wert für WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Setzt einen Wert für WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Speichert Basislinienfelder in die angegebene Basislinie für das gesamte Projekt. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Setzt die Basislinien-Speicherzeit. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Aktualisiert alle Arbeiten als abgeschlossen bis zu einem angegebenen Datum für das gesamte Projekt. |

