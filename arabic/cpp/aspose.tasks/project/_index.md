---
title: "Aspose::Tasks::Project class"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks لـ C++"
description: "يمثل مشروعًا."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/project/
---

## Project class

يمثل مشروعًا.

المشروع هو فئة مركزية في مكتبة Aspose.Tasks.

يمكن استخدام Project لقراءة أحد صيغ إدارة المشاريع المدعومة: MPP، MPT، MPX، XML.

لتحميل مستند موجود بأي من الصيغ المدعومة، مرّر اسم ملف أو تدفق إلى أحد مُنشئي Project. لإنشاء مشروع فارغ، استدعِ المُنشئ بدون معلمات.

استخدم أحد أشكال تحميل طريقة Save لحفظ المشروع بأي من صيغ Aspose::Tasks::Saving::SaveFileFormat: Primavera: P6 XML، PM XER؛ Microsoft Excel: XLSX، XML؛ Fixed Layout: PDF؛ Images: JPEG، PNG، BMP، TIFF، SVG؛ Text: TXT؛ Others: HTML.

المشروع يخزن معلومات على مستوى المشروع مثل Aspose::Tasks::Project::Views، Aspose::Tasks::Project::BuiltInProps، Aspose::Tasks::Project::CustomProps، وAspose::Tasks::Project::ExtendedAttributes. معظم هذه الكائنات يمكن الوصول إليها عبر الخصائص المقابلة لفئة Project.

المشروع هو كيان جذري يحتوي على نقاط دخول للتعامل مع كيانات المشروع الأخرى، مثل Aspose::Tasks::Task ، Aspose::Tasks::Resource ، Aspose::Tasks::ResourceAssignment ، Aspose::Tasks::ExtendedAttribute و Aspose::Tasks::Calendar .

يمكن الوصول إلى كيانات المشروع عبر مجموعات ذات نوع، على سبيل المثال Aspose::Tasks::Task::Children ، Aspose::Tasks::Project::Resources ، Aspose::Tasks::Project::ResourceAssignments ، إلخ.

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Project (13 overloads)](./project/) | يُنشئ مثيلًا جديدًا من فئة Project. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | يُعدد بشكل متكرر جميع مهام المشروع بما في ذلك المهمة الجذرية. |
| [Get](./get/) | يعيد القيمة التي تم ربط الخاصية بها في هذا الحاوية. |
| [get_ActualsInSync](./get_actualsinsync/) | يحصل على قيمة تشير إلى ما إذا كان ActualsInSync مُعيّنًا أم لا. |
| [get_AdminProject](./get_adminproject/) | يحصل على قيمة تشير إلى ما إذا كان AdminProject مُعيّنًا أم لا. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | يحصل على قيمة تشير إلى ما إذا كان AreEditableActualCosts مُعيّنًا أم لا. |
| [get_Author](./get_author/) | يحصل على قيمة Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | يحصل على قيمة تشير إلى ما إذا كان AutoAddNewResourcesAndTasks مُعيّنًا أم لا. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | يحصل على ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد. |
| [get_Autolink](./get_autolink/) | يحصل على قيمة تشير إلى ما إذا كان Autolink مُعيّنًا أم لا. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | يحصل على قيمة BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | يحصل على مجموعة الخصائص المدمجة للمشروع. |
| [get_CalculationMode](./get_calculationmode/) | يحصل على وضع الحساب للمشروع. يمكن أن يكون أحد قيم تعداد CalculationMode. |
| [get_Calendar](./get_calendar/) | يحصل على قيمة Calendar. |
| [get_Calendars](./get_calendars/) | يحصل على كائن CalendarCollection لهذا المثيل من Project. |
| [get_Category](./get_category/) | يحصل على قيمة Category. |
| [get_Comments](./get_comments/) | يحصل على قيمة Comments. |
| [get_Company](./get_company/) | يحصل على قيمة Company. |
| [get_CreationDate](./get_creationdate/) | يحصل على قيمة CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | يحصل على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | يحصل على قيمة CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | يحصل على قيمة CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | يحصل على قيمة CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | يحصل على قيمة CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | يحصل على قيمة CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | يحصل على قيمة CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | يحصل على قيمة CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | يحصل على مجموعة الخصائص المخصصة للمشروع. |
| [get_DateFormat](./get_dateformat/) | يحصل على قيمة DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | يحصل على قيمة DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | يحصل على قيمة DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | يحصل على قيمة DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | يحصل على قيمة DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | يحصل على قيمة DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | يحصل على قيمة DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | يحصل على قيمة DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | يحصل على قيمة DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | يحصل على العرض الافتراضي للمشروع. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | يحصل على نسخة من فئة WeekDayCollection التي تمثل مجموعة من أيام الأسبوع وساعات العمل الافتراضية للمشروع. |
| [get_DisplayOptions](./get_displayoptions/) | يحصل على نسخة من فئة ProjectDisplayOptions. |
| [get_DurationFormat](./get_durationformat/) | يحصل على قيمة DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | يحصل على قيمة EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | يحصل على كائن ExtendedAttributeDefinitionCollection. مجموعة تعريفات السمات الموسعة (الحقول المخصصة) المرتبطة بمشروع. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | يحصل على قيمة ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | يحصل على قيمة FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | يحصل على قيمة تشير إلى ما إذا كان FiscalYearStart مضبوطًا أم لا. |
| [get_FyStartDate](./get_fystartdate/) | يحصل على قيمة FyStartDate. |
| [get_Guid](./get_guid/) | يحصل على قيمة Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | يحصل على قيمة تشير إلى ما إذا كان HonorConstraints مضبوطًا أم لا. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | يحصل على قيمة HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | يحصل على قيمة تشير إلى ما إذا كان InsertedProjectsLikeSummary مضبوطًا أم لا. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | يحصل على قيمة تشير إلى ما إذا كان KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled مضبوطًا أم لا. |
| [get_Keywords](./get_keywords/) | يحصل على قيمة للخاصية Keywords. |
| [get_LastAuthor](./get_lastauthor/) | يحصل على قيمة للخاصية LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | يحصل على قيمة للخاصية LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | يحصل على قيمة للخاصية LastSaved. |
| [get_Manager](./get_manager/) | يحصل على قيمة للخاصية Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | يحصل على قيمة تشير إلى ما إذا كان MicrosoftProjectServerURL مضبوطًا أم لا. |
| [get_MinutesPerDay](./get_minutesperday/) | يحصل على قيمة للخاصية MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | يحصل على قيمة للخاصية MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsBack مضبوطًا أم لا. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | يحصل على قيمة تشير إلى ما إذا كان MoveCompletedEndsForward مضبوطًا أم لا. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsBack مضبوطًا أم لا. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | يحصل على قيمة تشير إلى ما إذا كان MoveRemainingStartsForward مضبوطًا أم لا. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | يحصل على قيمة تشير إلى ما إذا كان MultipleCriticalPaths مضبوطًا أم لا. |
| [get_Name](./get_name/) | يحصل على قيمة Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | يحصل على قيمة تشير إلى ما إذا كان NewTasksAreManual مضبوطًا أم لا. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | يحصل على قيمة تشير إلى ما إذا كان NewTasksEffortDriven مضبوطًا أم لا. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | يحصل على قيمة تشير إلى ما إذا كان NewTasksEstimated مضبوطًا أم لا. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | يحصل على قيمة للخاصية NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | يحصل على مجموعة تحتوي على كائنات من فئة OleObject المرتبطة أو المدمجة في ملف المشروع هذا. |
| [get_OutlineCodes](./get_outlinecodes/) | يحصل على كائن OutlineCodeDefinitionCollection. مجموعة تعريفات رموز المخطط المرتبطة بمشروع. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لمشروع يُقرأ من ملف Primavera. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | يحصل على قيمة تشير إلى ما إذا كان ProjectExternallyEdited مضبوطًا أم لا. |
| [get_RemoveFileProperties](./get_removefileproperties/) | يحصل على قيمة تشير إلى ما إذا كان RemoveFileProperties مضبوطًا أم لا. |
| [get_ResourceAssignments](./get_resourceassignments/) | يحصل على كائن ResourceAssignmentCollection. |
| [get_ResourceFilters](./get_resourcefilters/) | يحصل على جميع تعريفات الفلاتر المستندة إلى الموارد. ResourceFilters هي مجموعة من كائنات Filter. |
| [get_ResourceGroups](./get_resourcegroups/) | يحصل على جميع تعريفات المجموعات المستندة إلى الموارد. ResourceGroups هي مجموعة من كائنات Group. |
| [get_Resources](./get_resources/) | يحصل على كائن ResourceCollection. |
| [get_Revision](./get_revision/) | يحصل على قيمة Revision. |
| [get_RootTask](./get_roottask/) | يحصل على جذر شجرة المهام. |
| [get_SaveVersion](./get_saveversion/) | يحصل على قيمة SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | يحصل على قيمة تشير إلى ما إذا كان ScheduleFromStart مضبوطًا أم لا. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | يحصل على قيمة تشير إلى ما إذا كان ShowProjectSummaryTask مضبوطًا أم لا. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | يحصل على قيمة تشير إلى ما إذا كان SplitsInProgressTasks مضبوطًا أم لا. |
| [get_SpreadActualCost](./get_spreadactualcost/) | يحصل على قيمة تشير إلى ما إذا كان SpreadActualCost مضبوطًا أم لا. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | يحصل على قيمة تشير إلى ما إذا كان SpreadPercentComplete مضبوطًا أم لا. |
| [get_StartDate](./get_startdate/) | يحصل على قيمة StartDate. |
| [get_StatusDate](./get_statusdate/) | يحصل على قيمة StatusDate. |
| [get_Subject](./get_subject/) | يحصل على قيمة Subject. |
| [get_Tables](./get_tables/) | يحصل على قائمة من كائنات Table. |
| [get_TaskFilters](./get_taskfilters/) | يحصل على جميع تعريفات الفلاتر المستندة إلى المهام. TaskFilters هي مجموعة من كائنات Filter. |
| [get_TaskGroups](./get_taskgroups/) | يحصل على جميع تعريفات المجموعات المستندة إلى المهام. TaskGroups هي مجموعة من كائنات Group. |
| [get_TaskLinks](./get_tasklinks/) | يحصل على كائن TaskLinkCollection. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | يحصل على قيمة تشير إلى ما إذا كان TaskUpdatesResource مضبوطًا أم لا. |
| [get_Template](./get_template/) | يحصل على قيمة Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | يحصل على قيمة TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | يحصل على قيمة TimescaleStart. |
| [get_Title](./get_title/) | يحصل على قيمة Title. |
| [get_Uid](./get_uid/) | يحصل على قيمة Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | يحصل على قيمة تشير إلى ما إذا كان UpdateManuallyScheduledTasksWhenEditingLinks مضبوطًا أم لا. |
| [get_VbaProject](./get_vbaproject/) | يحصل على نسخة من الفئة VbaProject. |
| [get_Views](./get_views/) | يحصل على قائمة من كائنات View. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | يحصل على تعريف رمز WBS للمشروع. |
| [get_WeekStartDay](./get_weekstartday/) | يحصل على قيمة WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | يحصل على قيمة WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | يعيد وقت حفظ الخط الأساسي. |
| [GetDuration (3 overloads)](./getduration/) | يحصل على كائن Duration مع عدد الوحدات المحدد وتنسيق المدة الافتراضي الذي يتم تعريفه في إعدادات المشروع Prj::DurationFormat. |
| [GetPageCount (7 overloads)](./getpagecount/) | يعيد عدد الصفحات للمشروع ليتم عرضه باستخدام مقياس الوقت الافتراضي (Days). |
| [GetPredecessors](./getpredecessors/) | يعيد مجموعة من روابط المهام التي هي سابقة للمهمة المحددة. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | يحصل على معلومات ملف المشروع من الدفق. |
| [GetWork](./getwork/) | يحصل على كائن Duration مع القيمة المزدوجة المحددة وتنسيق العمل الافتراضي. |
| [Recalculate (2 overloads)](./recalculate/) | يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة. |
| [RecalculateResourceFields](./recalculateresourcefields/) | يعيد حساب Id و Start و Finish للموارد. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | يعيد حساب Start و Finish للموارد. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | يزيل تعيينات الموارد غير الصالحة من قائمة تعيينات موارد المشروع. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | يعيد ترقيم رمز WBS لجميع المهام. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | يعيد جدولة عمل المشروع غير المكتمل ليبدأ بعد تاريخ محدد. |
| [Save (5 overloads)](./save/) | يحفظ المشروع إلى دفق باستخدام خيارات الحفظ المحددة. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | يحفظ المشروع كقالب إلى دفق محدد. |
| [SaveReport (4 overloads)](./savereport/) | يحفظ تقرير نظرة عامة على المشروع إلى الدفق. |
| [SelectAllChildTasks](./selectallchildtasks/) | يجمع بشكل متكرر جميع المهام الفرعية للمهمة الجذرية. |
| [Set (2 overloads)](./set/) | يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية. |
| [set_ActualsInSync](./set_actualsinsync/) | يضبط قيمة تشير إلى ما إذا كان ActualsInSync مضبوطًا أم لا. |
| [set_AdminProject](./set_adminproject/) | يضبط قيمة تشير إلى ما إذا كان AdminProject مضبوطًا أم لا. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | يضبط قيمة تشير إلى ما إذا كان AreEditableActualCosts مضبوطًا أم لا. |
| [set_Author](./set_author/) | يضبط قيمة Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | يضبط قيمة تشير إلى ما إذا كان AutoAddNewResourcesAndTasks مضبوطًا أم لا. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | يضبط ما إذا كان يجب حساب تكلفة التعيين والتكلفة المتبقية تلقائيًا باستخدام عمل التعيين ومعدلات الموارد. |
| [set_Autolink](./set_autolink/) | يضبط قيمة تشير إلى ما إذا كان Autolink مُفعلاً أم لا. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | يضبط قيمة BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | يضبط وضع الحساب للمشروع. يمكن أن يكون أحد قيم تعداد CalculationMode. |
| [set_Calendar](./set_calendar/) | يضبط قيمة Calendar . |
| [set_Category](./set_category/) | يضبط قيمة الفئة. |
| [set_Comments](./set_comments/) | يضبط قيمة التعليقات. |
| [set_Company](./set_company/) | يضبط قيمة الشركة. |
| [set_CreationDate](./set_creationdate/) | يضبط قيمة تاريخ الإنشاء. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | يضبط قيمة حد الفاصل الزمني الحرج. |
| [set_CurrencyCode](./set_currencycode/) | يضبط قيمة رمز العملة. |
| [set_CurrencyDigits](./set_currencydigits/) | يضبط قيمة أرقام العملة. |
| [set_CurrencySymbol](./set_currencysymbol/) | يضبط قيمة رمز العملة. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | يضبط قيمة موضع رمز العملة. |
| [set_CurrentDate](./set_currentdate/) | يضبط قيمة التاريخ الحالي. |
| [set_CustomDateFormat](./set_customdateformat/) | يضبط قيمة تنسيق التاريخ المخصص. |
| [set_DateFormat](./set_dateformat/) | يضبط قيمة تنسيق التاريخ. |
| [set_DaysPerMonth](./set_dayspermonth/) | يضبط قيمة الأيام في الشهر. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | يضبط قيمة وقت الانتهاء الافتراضي. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | يضبط قيمة تراكم التكلفة الثابتة الافتراضية. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | يضبط قيمة معدل العمل الإضافي الافتراضي. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | يضبط قيمة المعدل القياسي الافتراضي. |
| [set_DefaultStartTime](./set_defaultstarttime/) | يضبط قيمة وقت البدء الافتراضي. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | يضبط قيمة طريقة القيمة المكتسبة الافتراضية للمهمة. |
| [set_DefaultTaskType](./set_defaulttasktype/) | يضبط قيمة نوع المهمة الافتراضي. |
| [set_DefaultView](./set_defaultview/) | يضبط العرض الافتراضي للمشروع. |
| [set_DurationFormat](./set_durationformat/) | يضبط قيمة DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | يضبط قيمة EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | يضبط قيمة ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | يضبط قيمة FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | يضبط قيمة تشير إلى ما إذا كان FiscalYearStart معينًا أم لا. |
| [set_FyStartDate](./set_fystartdate/) | يضبط قيمة FyStartDate. |
| [set_Guid](./set_guid/) | يحدد قيمة Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | يضبط قيمة تشير إلى ما إذا كان HonorConstraints معينًا أم لا. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | يضبط قيمة HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | يضبط قيمة تشير إلى ما إذا كان InsertedProjectsLikeSummary معينًا أم لا. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | يضبط قيمة تشير إلى ما إذا كان KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled معينًا أم لا. |
| [set_Keywords](./set_keywords/) | يضبط قيمة Keywords. |
| [set_LastAuthor](./set_lastauthor/) | يضبط قيمة LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | يضبط قيمة LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | يضبط قيمة LastSaved. |
| [set_Manager](./set_manager/) | يضبط قيمة Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | يضبط قيمة تشير إلى ما إذا كان MicrosoftProjectServerURL معينًا أم لا. |
| [set_MinutesPerDay](./set_minutesperday/) | يضبط قيمة MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | يضبط قيمة MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | يضبط قيمة تشير إلى ما إذا كان MoveCompletedEndsBack معينًا أم لا. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | يضبط قيمة تشير إلى ما إذا كان MoveCompletedEndsForward معينًا أم لا. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | يضبط قيمة تشير إلى ما إذا كان MoveRemainingStartsBack معينًا أم لا. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | يضبط قيمة تشير إلى ما إذا كان MoveRemainingStartsForward معينًا أم لا. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | يضبط قيمة تشير إلى ما إذا كان MultipleCriticalPaths معينًا أم لا. |
| [set_Name](./set_name/) | يحدد قيمة Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | يضبط قيمة تشير إلى ما إذا كان NewTasksAreManual معينًا أم لا. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | يضبط قيمة تشير إلى ما إذا كان NewTasksEffortDriven معينًا أم لا. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | يضبط قيمة تشير إلى ما إذا كان NewTasksEstimated مضبوطًا أم لا. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | يضبط قيمة لـ NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | يضبط قيمة تشير إلى ما إذا كان ProjectExternallyEdited مضبوطًا أم لا. |
| [set_RemoveFileProperties](./set_removefileproperties/) | يضبط قيمة تشير إلى ما إذا كان RemoveFileProperties مضبوطًا أم لا. |
| [set_Revision](./set_revision/) | يضبط قيمة لـ Revision. |
| [set_SaveVersion](./set_saveversion/) | يضبط قيمة لـ SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | يضبط قيمة تشير إلى ما إذا كان ScheduleFromStart مضبوطًا أم لا. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | يضبط قيمة تشير إلى ما إذا كان ShowProjectSummaryTask مضبوطًا أم لا. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | يضبط قيمة تشير إلى ما إذا كان SplitsInProgressTasks مضبوطًا أم لا. |
| [set_SpreadActualCost](./set_spreadactualcost/) | يضبط قيمة تشير إلى ما إذا كان SpreadActualCost مضبوطًا أم لا. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | يضبط قيمة تشير إلى ما إذا كان SpreadPercentComplete مضبوطًا أم لا. |
| [set_StartDate](./set_startdate/) | يضبط قيمة لـ StartDate. |
| [set_StatusDate](./set_statusdate/) | يضبط قيمة لـ StatusDate. |
| [set_Subject](./set_subject/) | يضبط قيمة لـ Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | يضبط قيمة تشير إلى ما إذا كان TaskUpdatesResource مضبوطًا أم لا. |
| [set_Template](./set_template/) | يضبط قيمة لـ Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | يضبط قيمة لـ TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | يضبط قيمة لـ TimescaleStart. |
| [set_Title](./set_title/) | يضبط قيمة لـ Title. |
| [set_Uid](./set_uid/) | يضبط قيمة Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | يضبط قيمة تشير إلى ما إذا كان UpdateManuallyScheduledTasksWhenEditingLinks مضبوطًا أم لا. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | يضبط تعريف رمز WBS للمشروع. |
| [set_WeekStartDay](./set_weekstartday/) | يضبط قيمة لـ WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | يضبط قيمة لـ WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | يحفظ حقول الخط الأساسي إلى الخط الأساسي المحدد لكامل المشروع. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | يضبط وقت حفظ الخط الأساسي. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للمشروع بأكمله. |

