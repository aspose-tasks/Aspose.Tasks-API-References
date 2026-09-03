---
title: "класс Aspose::Tasks::Project"
linktitle: "Проект"
articleTitle: "Проект"
second_title: "Aspose.Tasks для C++"
description: "Представляет проект."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/project/
---

## Project class

Представляет проект.

Проект является центральным классом в библиотеке Aspose.Tasks.

Можно использовать Project для чтения одного из поддерживаемых форматов управления проектами: MPP, MPT, MPX, XML.

Чтобы загрузить существующий документ в любом из поддерживаемых форматов, передайте имя файла или поток в один из конструкторов Project. Чтобы создать пустой проект, вызовите конструктор без параметров.

Используйте одну из перегрузок метода Save, чтобы сохранить проект в любом из форматов Aspose::Tasks::Saving::SaveFileFormat: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Фиксированный макет: PDF; Изображения: JPEG, PNG, BMP, TIFF, SVG; Текст: TXT; Другие: HTML.

Project хранит информацию, охватывающую весь проект, такую как Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps и Aspose::Tasks::Project::ExtendedAttributes. Большинство этих объектов доступны через соответствующие свойства класса Project.

Project является корневой сущностью, содержащей точки входа для манипулирования другими сущностями проекта, такими как Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute и Aspose::Tasks::Calendar.

Сущности Project могут быть доступны через типизированные коллекции, например Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments и т.д.

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Project (13 overloads)](./project/) | Инициализирует новый экземпляр класса Project. |

## Методы

| Имя | Описание |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Копирует основные данные и свойства проекта в другой проект. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Рекурсивно перечисляет все задачи проекта, включая корневую задачу. |
| [Get](./get/) | Возвращает значение, к которому свойство сопоставлено в этом контейнере. |
| [get_ActualsInSync](./get_actualsinsync/) | Возвращает значение, указывающее, установлен ли ActualsInSync. |
| [get_AdminProject](./get_adminproject/) | Возвращает значение, указывающее, установлен ли AdminProject. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Возвращает значение, указывающее, установлен ли AreEditableActualCosts. |
| [get_Author](./get_author/) | Возвращает значение свойства Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Возвращает значение, указывающее, установлен ли AutoAddNewResourcesAndTasks. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Возвращает, следует ли автоматически рассчитывать стоимость назначения и оставшуюся стоимость, используя работу назначения и ставки ресурсов. |
| [get_Autolink](./get_autolink/) | Возвращает значение, указывающее, установлен ли Autolink. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Возвращает значение свойства BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Возвращает коллекцию встроенных свойств проекта. |
| [get_CalculationMode](./get_calculationmode/) | Возвращает режим расчётов проекта. Может быть одним из значений перечисления CalculationMode. |
| [get_Calendar](./get_calendar/) | Получает значение Calendar. |
| [get_Calendars](./get_calendars/) | Возвращает объект CalendarCollection данного экземпляра Project. |
| [get_Category](./get_category/) | Возвращает значение свойства Category. |
| [get_Comments](./get_comments/) | Возвращает значение свойства Comments. |
| [get_Company](./get_company/) | Возвращает значение свойства Company. |
| [get_CreationDate](./get_creationdate/) | Возвращает значение свойства CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Возвращает коллекцию, содержащую список критических задач, составляющих критический путь этого проекта. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Получает значение CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Получает значение CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Получает значение CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Получает значение CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Получает значение CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Получает значение CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Получает значение CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Получает коллекцию пользовательских свойств проекта. |
| [get_DateFormat](./get_dateformat/) | Получает значение DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Получает значение DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Получает значение DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Получает значение DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Получает значение DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Получает значение DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Получает значение DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Получает значение DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Получает значение DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Получает представление проекта по умолчанию. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Получает экземпляр класса WeekDayCollection, который представляет коллекцию стандартных рабочих дней недели проекта и их рабочее время. |
| [get_DisplayOptions](./get_displayoptions/) | Получает экземпляр класса ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | Получает значение DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Получает значение EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Получает объект ExtendedAttributeDefinitionCollection. Коллекция определений расширенных атрибутов (пользовательских полей), связанных с проектом. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Получает значение ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Получает значение FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Получает значение, указывающее, установлен ли FiscalYearStart, или нет. |
| [get_FyStartDate](./get_fystartdate/) | Получает значение FyStartDate. |
| [get_Guid](./get_guid/) | Получает значение Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Получает значение, указывающее, установлен ли HonorConstraints, или нет. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Получает значение HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Получает значение, указывающее, установлен ли InsertedProjectsLikeSummary, или нет. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Получает значение, указывающее, установлен ли KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, или нет. |
| [get_Keywords](./get_keywords/) | Получает значение Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Получает значение LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Получает значение LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Получает значение LastSaved. |
| [get_Manager](./get_manager/) | Получает значение Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Получает значение, указывающее, установлен ли MicrosoftProjectServerURL, или нет. |
| [get_MinutesPerDay](./get_minutesperday/) | Получает значение MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Получает значение MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Получает значение, указывающее, установлен ли MoveCompletedEndsBack, или нет. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Получает значение, указывающее, установлен ли MoveCompletedEndsForward, или нет. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Получает значение, указывающее, установлен ли MoveRemainingStartsBack, или нет. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Получает значение, указывающее, установлен ли MoveRemainingStartsForward, или нет. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Получает значение, указывающее, установлен ли MultipleCriticalPaths, или нет. |
| [get_Name](./get_name/) | Получает значение Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Получает значение, указывающее, установлен ли NewTasksAreManual, или нет. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Получает значение, указывающее, установлен ли NewTasksEffortDriven, или нет. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Получает значение, указывающее, установлен ли NewTasksEstimated, или нет. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Получает значение NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Получает коллекцию, содержащую экземпляры класса OleObject, которые связаны или внедрены в этот файл проекта. |
| [get_OutlineCodes](./get_outlinecodes/) | Получает объект OutlineCodeDefinitionCollection. Коллекция определений контурных кодов, связанных с проектом. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Получает объект, содержащий свойства, специфичные для Primavera, для проекта, считанного из файла Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Получает значение, указывающее, установлен ли ProjectExternallyEdited. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Получает значение, указывающее, установлен ли RemoveFileProperties. |
| [get_ResourceAssignments](./get_resourceassignments/) | Получает объект ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | Получает все определения фильтров, основанных на ресурсах. ResourceFilters — это коллекция объектов Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | Получает все определения групп, основанных на ресурсах. ResourceGroups — это коллекция объектов Group. |
| [get_Resources](./get_resources/) | Получает объект ResourceCollection. |
| [get_Revision](./get_revision/) | Получает значение Revision. |
| [get_RootTask](./get_roottask/) | Получает корень дерева задач. |
| [get_SaveVersion](./get_saveversion/) | Получает значение SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Получает значение, указывающее, установлен ли ScheduleFromStart. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Получает значение, указывающее, установлен ли ShowProjectSummaryTask. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Получает значение, указывающее, установлен ли SplitsInProgressTasks. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Получает значение, указывающее, установлен ли SpreadActualCost. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Получает значение, указывающее, установлен ли SpreadPercentComplete. |
| [get_StartDate](./get_startdate/) | Получает значение StartDate. |
| [get_StatusDate](./get_statusdate/) | Получает значение StatusDate. |
| [get_Subject](./get_subject/) | Получает значение Subject. |
| [get_Tables](./get_tables/) | Получает список объектов Table. |
| [get_TaskFilters](./get_taskfilters/) | Получает все определения фильтров, основанных на задачах. TaskFilters — это коллекция объектов Filter. |
| [get_TaskGroups](./get_taskgroups/) | Получает все определения групп, основанных на задачах. TaskGroups — это коллекция объектов Group. |
| [get_TaskLinks](./get_tasklinks/) | Получает объект TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Получает значение, указывающее, установлен ли TaskUpdatesResource. |
| [get_Template](./get_template/) | Получает значение Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Получает значение TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Получает значение TimescaleStart. |
| [get_Title](./get_title/) | Получает значение Title. |
| [get_Uid](./get_uid/) | Получает значение Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Получает значение, указывающее, установлен ли UpdateManuallyScheduledTasksWhenEditingLinks. |
| [get_VbaProject](./get_vbaproject/) | Получает экземпляр класса VbaProject. |
| [get_Views](./get_views/) | Получает список объектов View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Получает определение кода WBS для проекта. |
| [get_WeekStartDay](./get_weekstartday/) | Получает значение WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Получает значение WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Возвращает время сохранения базовой линии. |
| [GetDuration (3 overloads)](./getduration/) | Получает объект Duration с указанным количеством единиц и форматом длительности по умолчанию, определённым в настройках проекта Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | Возвращает количество страниц проекта, которое будет отрисовано, используя масштаб по умолчанию Timescale (Days). |
| [GetPredecessors](./getpredecessors/) | Возвращает коллекцию связей задач, которые являются предшественниками указанной задачи. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Получает информацию о файле проекта из потока. |
| [GetWork](./getwork/) | Получает объект Duration с указанным двойным значением и форматом работы по умолчанию. |
| [Recalculate (2 overloads)](./recalculate/) | Перепланирует идентификаторы всех задач проекта, уровни структуры, даты начала/завершения, устанавливает ранние/поздние даты, рассчитывает запасы времени, работу и поля стоимости. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Пересчитывает Id, Start и Finish ресурсов. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Пересчитывает Start и Finish ресурсов. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Убирает недействительные назначения ресурсов из списка назначений ресурсов проекта. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Перенумеровывает код WBS всех задач. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Перепланирует незавершённую работу проекта, чтобы она началась после указанной даты. |
| [Save (5 overloads)](./save/) | Сохраняет проект в поток, используя указанные параметры сохранения. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Сохраняет проект как шаблон в указанный поток. |
| [SaveReport (4 overloads)](./savereport/) | Сохраняет обзорный отчёт проекта в поток. |
| [SelectAllChildTasks](./selectallchildtasks/) | Рекурсивно собирает все дочерние задачи корневой задачи. |
| [Set (2 overloads)](./set/) | Отображает указанное свойство на указанное значение в этом контейнере. |
| [set_ActualsInSync](./set_actualsinsync/) | Устанавливает значение, указывающее, установлен ли ActualsInSync. |
| [set_AdminProject](./set_adminproject/) | Устанавливает значение, указывающее, установлен ли AdminProject, или нет. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Устанавливает значение, указывающее, установлен ли AreEditableActualCosts, или нет. |
| [set_Author](./set_author/) | Устанавливает значение Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Устанавливает значение, указывающее, установлен ли AutoAddNewResourcesAndTasks, или нет. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Устанавливает, следует ли автоматически рассчитывать стоимость назначения и оставшуюся стоимость, используя работу назначения и ставки ресурсов. |
| [set_Autolink](./set_autolink/) | Устанавливает значение, указывающее, установлен ли Autolink, или нет. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Устанавливает значение BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Устанавливает режим расчёта проекта. Может быть одним из значений перечисления CalculationMode. |
| [set_Calendar](./set_calendar/) | Устанавливает значение Calendar . |
| [set_Category](./set_category/) | Устанавливает значение Category. |
| [set_Comments](./set_comments/) | Устанавливает значение Comments. |
| [set_Company](./set_company/) | Устанавливает значение Company. |
| [set_CreationDate](./set_creationdate/) | Устанавливает значение CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Устанавливает значение CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Устанавливает значение CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Устанавливает значение CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Устанавливает значение CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Устанавливает значение CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Устанавливает значение CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Устанавливает значение CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Устанавливает значение DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Устанавливает значение DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Устанавливает значение DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Устанавливает значение DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Устанавливает значение DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Устанавливает значение DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Устанавливает значение DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Устанавливает значение DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Устанавливает значение DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Устанавливает представление по умолчанию проекта. |
| [set_DurationFormat](./set_durationformat/) | Устанавливает значение DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Устанавливает значение EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Устанавливает значение ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Устанавливает значение FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Устанавливает значение, указывающее, установлен ли FiscalYearStart, или нет. |
| [set_FyStartDate](./set_fystartdate/) | Устанавливает значение FyStartDate. |
| [set_Guid](./set_guid/) | Устанавливает значение Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Устанавливает значение, указывающее, установлен ли HonorConstraints, или нет. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Устанавливает значение HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Устанавливает значение, указывающее, установлен ли InsertedProjectsLikeSummary, или нет. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Устанавливает значение, указывающее, установлен ли KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, или нет. |
| [set_Keywords](./set_keywords/) | Устанавливает значение Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Устанавливает значение LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Устанавливает значение LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Устанавливает значение LastSaved. |
| [set_Manager](./set_manager/) | Устанавливает значение Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Устанавливает значение, указывающее, установлен ли MicrosoftProjectServerURL, или нет. |
| [set_MinutesPerDay](./set_minutesperday/) | Устанавливает значение MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Устанавливает значение MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Устанавливает значение, указывающее, установлен ли MoveCompletedEndsBack, или нет. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Устанавливает значение, указывающее, установлен ли MoveCompletedEndsForward, или нет. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Устанавливает значение, указывающее, установлен ли MoveRemainingStartsBack, или нет. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Устанавливает значение, указывающее, установлен ли MoveRemainingStartsForward, или нет. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Устанавливает значение, указывающее, установлен ли MultipleCriticalPaths, или нет. |
| [set_Name](./set_name/) | Устанавливает значение Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Устанавливает значение, указывающее, установлен ли NewTasksAreManual, или нет. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Устанавливает значение, указывающее, установлен ли NewTasksEffortDriven, или нет. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Устанавливает значение, указывающее, установлен ли NewTasksEstimated, или нет. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Устанавливает значение NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Устанавливает значение, указывающее, установлен ли ProjectExternallyEdited, или нет. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Устанавливает значение, указывающее, установлен ли RemoveFileProperties, или нет. |
| [set_Revision](./set_revision/) | Устанавливает значение Revision. |
| [set_SaveVersion](./set_saveversion/) | Устанавливает значение SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Устанавливает значение, указывающее, установлен ли ScheduleFromStart, или нет. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Устанавливает значение, указывающее, установлен ли ShowProjectSummaryTask, или нет. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Устанавливает значение, указывающее, установлен ли SplitsInProgressTasks, или нет. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Устанавливает значение, указывающее, установлен ли SpreadActualCost, или нет. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Устанавливает значение, указывающее, установлен ли SpreadPercentComplete, или нет. |
| [set_StartDate](./set_startdate/) | Устанавливает значение StartDate. |
| [set_StatusDate](./set_statusdate/) | Устанавливает значение StatusDate. |
| [set_Subject](./set_subject/) | Устанавливает значение Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Устанавливает значение, указывающее, установлен ли TaskUpdatesResource, или нет. |
| [set_Template](./set_template/) | Устанавливает значение Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Устанавливает значение TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Устанавливает значение TimescaleStart. |
| [set_Title](./set_title/) | Устанавливает значение Title. |
| [set_Uid](./set_uid/) | Устанавливает значение Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Устанавливает значение, указывающее, установлен ли UpdateManuallyScheduledTasksWhenEditingLinks, или нет. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Устанавливает определение кода WBS для проекта. |
| [set_WeekStartDay](./set_weekstartday/) | Устанавливает значение WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Устанавливает значение WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Сохраняет поля базового плана в указанный базовый план для всего проекта. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Устанавливает время сохранения базового плана. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Обновляет всю работу как выполненную до указанной даты для всего проекта. |

