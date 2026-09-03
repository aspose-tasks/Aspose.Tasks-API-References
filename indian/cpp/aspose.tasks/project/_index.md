---
title: "Aspose::Tasks::Project क्लास"
linktitle: "प्रोजेक्ट"
articleTitle: "प्रोजेक्ट"
second_title: "Aspose.Tasks C++ के लिए"
description: "किसी प्रोजेक्ट का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/project/
---

## Project class

किसी प्रोजेक्ट का प्रतिनिधित्व करता है।

प्रोजेक्ट Aspose.Tasks लाइब्रेरी में एक केंद्रीय क्लास है।

आप Project का उपयोग करके समर्थित प्रोजेक्ट मैनेजमेंट फ़ॉर्मैट्स में से एक, जैसे MPP, MPT, MPX, XML, पढ़ सकते हैं।

समर्थित फ़ॉर्मैट्स में से किसी भी फ़ॉर्मैट में मौजूदा दस्तावेज़ लोड करने के लिए, फ़ाइल नाम या स्ट्रीम को Project कन्स्ट्रक्टर्स में से किसी एक में पास करें। एक खाली प्रोजेक्ट बनाने के लिए, पैरामीटर‑लेस कन्स्ट्रक्टर को कॉल करें।

प्रोजेक्ट को किसी भी Aspose::Tasks::Saving::SaveFileFormat फ़ॉर्मैट में सहेजने के लिए Save मेथड के ओवरलोड्स में से एक का उपयोग करें: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

Project प्रोजेक्ट‑व्यापी जानकारी जैसे Aspose::Tasks::Project::Views, Aspose::Tasks::Project::BuiltInProps, Aspose::Tasks::Project::CustomProps, और Aspose::Tasks::Project::ExtendedAttributes को संग्रहीत करता है। इन वस्तुओं में से अधिकांश Project क्लास की संबंधित प्रॉपर्टीज़ के माध्यम से उपलब्ध हैं।

Project एक मूल इकाई है जो अन्य प्रोजेक्ट इकाइयों, जैसे Aspose::Tasks::Task, Aspose::Tasks::Resource, Aspose::Tasks::ResourceAssignment, Aspose::Tasks::ExtendedAttribute और Aspose::Tasks::Calendar, को हेरफेर करने के लिए एंट्री पॉइंट्स प्रदान करती है।

Project इकाइयों तक टाइप्ड कलेक्शन्स के माध्यम से पहुंचा जा सकता है, उदाहरण के लिए Aspose::Tasks::Task::Children, Aspose::Tasks::Project::Resources, Aspose::Tasks::Project::ResourceAssignments आदि।

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Project (13 overloads)](./project/) | Project क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | प्रोजेक्ट के मुख्य डेटा और प्रॉपर्टीज़ को दूसरे प्रोजेक्ट में कॉपी करता है। |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | रूट टास्क सहित प्रोजेक्ट के सभी टास्क को पुनरावर्ती रूप से सूचीबद्ध करता है। |
| [Get](./get/) | इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है। |
| [get_ActualsInSync](./get_actualsinsync/) | यह बताने वाला मान प्राप्त करता है कि ActualsInSync सेट है या नहीं। |
| [get_AdminProject](./get_adminproject/) | यह बताने वाला मान प्राप्त करता है कि AdminProject सेट है या नहीं। |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | यह बताने वाला मान प्राप्त करता है कि AreEditableActualCosts सेट है या नहीं। |
| [get_Author](./get_author/) | Author का मान प्राप्त करता है। |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | यह बताने वाला मान प्राप्त करता है कि AutoAddNewResourcesAndTasks सेट है या नहीं। |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | यह प्राप्त करता है कि असाइनमेंट लागत और शेष लागत को असाइनमेंट के कार्य और रिसोर्स रेट्स का उपयोग करके स्वतः गणना किया जाना चाहिए या नहीं। |
| [get_Autolink](./get_autolink/) | यह बताने वाला मान प्राप्त करता है कि Autolink सेट है या नहीं। |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | BaselineForEarnedValue का मान प्राप्त करता है। |
| [get_BuiltInProps](./get_builtinprops/) | प्रोजेक्ट की बिल्ट‑इन प्रॉपर्टीज़ कलेक्शन प्राप्त करता है। |
| [get_CalculationMode](./get_calculationmode/) | प्रोजेक्ट का कैलकुलेशन मोड प्राप्त करता है। यह CalculationMode एनेमरेशन के मानों में से एक हो सकता है। |
| [get_Calendar](./get_calendar/) | एक मान प्राप्त करता है Calendar। |
| [get_Calendars](./get_calendars/) | इस Project इंस्टेंस का CalendarCollection ऑब्जेक्ट प्राप्त करता है। |
| [get_Category](./get_category/) | Category का मान प्राप्त करता है। |
| [get_Comments](./get_comments/) | Comments का मान प्राप्त करता है। |
| [get_Company](./get_company/) | Company का मान प्राप्त करता है। |
| [get_CreationDate](./get_creationdate/) | CreationDate का मान प्राप्त करता है। |
| [get_CriticalPath](./get_criticalpath/) | एक कलेक्शन प्राप्त करता है जिसमें उन Critical टास्क की सूची होती है जो इस प्रोजेक्ट के Critical Path को बनाते हैं। |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | CriticalSlackLimit का मान प्राप्त करता है। |
| [get_CurrencyCode](./get_currencycode/) | CurrencyCode का मान प्राप्त करता है। |
| [get_CurrencyDigits](./get_currencydigits/) | CurrencyDigits का मान प्राप्त करता है। |
| [get_CurrencySymbol](./get_currencysymbol/) | CurrencySymbol का मान प्राप्त करता है। |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | CurrencySymbolPosition का मान प्राप्त करता है। |
| [get_CurrentDate](./get_currentdate/) | CurrentDate का मान प्राप्त करता है। |
| [get_CustomDateFormat](./get_customdateformat/) | CustomDateFormat का मान प्राप्त करता है। |
| [get_CustomProps](./get_customprops/) | प्रोजेक्ट की कस्टम प्रॉपर्टीज़ संग्रह प्राप्त करता है। |
| [get_DateFormat](./get_dateformat/) | DateFormat का मान प्राप्त करता है। |
| [get_DaysPerMonth](./get_dayspermonth/) | DaysPerMonth का मान प्राप्त करता है। |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | DefaultFinishTime का मान प्राप्त करता है। |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | DefaultFixedCostAccrual का मान प्राप्त करता है। |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | DefaultOvertimeRate का मान प्राप्त करता है। |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | DefaultStandardRate का मान प्राप्त करता है। |
| [get_DefaultStartTime](./get_defaultstarttime/) | DefaultStartTime का मान प्राप्त करता है। |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | DefaultTaskEVMethod का मान प्राप्त करता है। |
| [get_DefaultTaskType](./get_defaulttasktype/) | DefaultTaskType का मान प्राप्त करता है। |
| [get_DefaultView](./get_defaultview/) | प्रोजेक्ट का डिफ़ॉल्ट व्यू प्राप्त करता है। |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | WeekDayCollection क्लास का इंस्टेंस प्राप्त करता है जो प्रोजेक्ट के डिफ़ॉल्ट सप्ताह के कार्य दिवसों और कार्य समयों का संग्रह दर्शाता है। |
| [get_DisplayOptions](./get_displayoptions/) | ProjectDisplayOptions क्लास का एक इंस्टेंस प्राप्त करता है। |
| [get_DurationFormat](./get_durationformat/) | DurationFormat का मान प्राप्त करता है। |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod का मान प्राप्त करता है। |
| [get_ExtendedAttributes](./get_extendedattributes/) | ExtendedAttributeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़ी विस्तारित एट्रिब्यूट (कस्टम फ़ील्ड) परिभाषाओं का संग्रह। |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | ExtendedCreationDate का मान प्राप्त करता है। |
| [get_FinishDate](./get_finishdate/) | FinishDate का मान प्राप्त करता है। |
| [get_FiscalYearStart](./get_fiscalyearstart/) | FiscalYearStart सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_FyStartDate](./get_fystartdate/) | FyStartDate का मान प्राप्त करता है। |
| [get_Guid](./get_guid/) | Guid का मान प्राप्त करता है। |
| [get_HonorConstraints](./get_honorconstraints/) | HonorConstraints सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_HyperlinkBase](./get_hyperlinkbase/) | HyperlinkBase का मान प्राप्त करता है। |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | InsertedProjectsLikeSummary सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_Keywords](./get_keywords/) | Keywords का मान प्राप्त करता है। |
| [get_LastAuthor](./get_lastauthor/) | LastAuthor का मान प्राप्त करता है। |
| [get_LastPrinted](./get_lastprinted/) | LastPrinted का मान प्राप्त करता है। |
| [get_LastSaved](./get_lastsaved/) | LastSaved का मान प्राप्त करता है। |
| [get_Manager](./get_manager/) | Manager का मान प्राप्त करता है। |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | MicrosoftProjectServerURL सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_MinutesPerDay](./get_minutesperday/) | MinutesPerDay का मान प्राप्त करता है। |
| [get_MinutesPerWeek](./get_minutesperweek/) | MinutesPerWeek का मान प्राप्त करता है। |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | MoveCompletedEndsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | MoveCompletedEndsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | MoveRemainingStartsBack सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | MoveRemainingStartsForward सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | MultipleCriticalPaths सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_Name](./get_name/) | Name का मान प्राप्त करता है। |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | NewTasksAreManual सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | NewTasksEffortDriven सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_NewTasksEstimated](./get_newtasksestimated/) | NewTasksEstimated सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | NewTaskStartDate का मान प्राप्त करता है। |
| [get_OleObjects](./get_oleobjects/) | OleObject क्लास के उन इंस्टेंसों की संग्रह प्राप्त करता है जो इस प्रोजेक्ट फ़ाइल से लिंक या एम्बेड किए गए हैं। |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeDefinitionCollection ऑब्जेक्ट प्राप्त करता है। प्रोजेक्ट से जुड़े आउटलाइन कोड परिभाषाओं का संग्रह। |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera फ़ाइल से पढ़े गए प्रोजेक्ट के लिए Primavera-विशिष्ट गुणों वाले ऑब्जेक्ट को प्राप्त करता है। |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | यह दर्शाने वाला मान प्राप्त करता है कि ProjectExternallyEdited सेट है या नहीं। |
| [get_RemoveFileProperties](./get_removefileproperties/) | यह दर्शाने वाला मान प्राप्त करता है कि RemoveFileProperties सेट है या नहीं। |
| [get_ResourceAssignments](./get_resourceassignments/) | ResourceAssignmentCollection ऑब्जेक्ट को प्राप्त करता है। |
| [get_ResourceFilters](./get_resourcefilters/) | सभी रिसोर्स-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। ResourceFilters फ़िल्टर ऑब्जेक्ट्स का एक संग्रह है। |
| [get_ResourceGroups](./get_resourcegroups/) | सभी रिसोर्स-आधारित समूह परिभाषाएँ प्राप्त करता है। ResourceGroups समूह ऑब्जेक्ट्स का एक संग्रह है। |
| [get_Resources](./get_resources/) | ResourceCollection ऑब्जेक्ट को प्राप्त करता है। |
| [get_Revision](./get_revision/) | Revision का मान प्राप्त करता है। |
| [get_RootTask](./get_roottask/) | टास्क ट्री की जड़ (रूट) को प्राप्त करता है। |
| [get_SaveVersion](./get_saveversion/) | SaveVersion का मान प्राप्त करता है। |
| [get_ScheduleFromStart](./get_schedulefromstart/) | यह दर्शाने वाला मान प्राप्त करता है कि ScheduleFromStart सेट है या नहीं। |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | यह दर्शाने वाला मान प्राप्त करता है कि ShowProjectSummaryTask सेट है या नहीं। |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | यह दर्शाने वाला मान प्राप्त करता है कि SplitsInProgressTasks सेट है या नहीं। |
| [get_SpreadActualCost](./get_spreadactualcost/) | यह दर्शाने वाला मान प्राप्त करता है कि SpreadActualCost सेट है या नहीं। |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | यह दर्शाने वाला मान प्राप्त करता है कि SpreadPercentComplete सेट है या नहीं। |
| [get_StartDate](./get_startdate/) | StartDate का मान प्राप्त करता है। |
| [get_StatusDate](./get_statusdate/) | StatusDate का मान प्राप्त करता है। |
| [get_Subject](./get_subject/) | Subject का मान प्राप्त करता है। |
| [get_Tables](./get_tables/) | Table ऑब्जेक्ट्स की सूची प्राप्त करता है। |
| [get_TaskFilters](./get_taskfilters/) | सभी टास्क-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। TaskFilters फ़िल्टर ऑब्जेक्ट्स का एक संग्रह है। |
| [get_TaskGroups](./get_taskgroups/) | सभी टास्क-आधारित समूह परिभाषाएँ प्राप्त करता है। TaskGroups समूह ऑब्जेक्ट्स का एक संग्रह है। |
| [get_TaskLinks](./get_tasklinks/) | TaskLinkCollection ऑब्जेक्ट को प्राप्त करता है। |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | यह दर्शाने वाला मान प्राप्त करता है कि TaskUpdatesResource सेट है या नहीं। |
| [get_Template](./get_template/) | Template का मान प्राप्त करता है। |
| [get_TimescaleFinish](./get_timescalefinish/) | TimescaleFinish का मान प्राप्त करता है। |
| [get_TimescaleStart](./get_timescalestart/) | TimescaleStart का मान प्राप्त करता है। |
| [get_Title](./get_title/) | Title का मान प्राप्त करता है। |
| [get_Uid](./get_uid/) | Uid का मान प्राप्त करता है। |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | UpdateManuallyScheduledTasksWhenEditingLinks सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_VbaProject](./get_vbaproject/) | VbaProject क्लास का एक उदाहरण प्राप्त करता है। |
| [get_Views](./get_views/) | View ऑब्जेक्ट्स की सूची प्राप्त करता है। |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | प्रोजेक्ट के लिए WBS कोड परिभाषा प्राप्त करता है। |
| [get_WeekStartDay](./get_weekstartday/) | WeekStartDay का मान प्राप्त करता है। |
| [get_WorkFormat](./get_workformat/) | WorkFormat का मान प्राप्त करता है। |
| [GetBaselineSaveTime](./getbaselinesavetime/) | बेसलाइन सहेजने का समय लौटाता है। |
| [GetDuration (3 overloads)](./getduration/) | Duration ऑब्जेक्ट प्राप्त करता है जिसमें निर्दिष्ट इकाइयों की संख्या और डिफ़ॉल्ट अवधि फ़ॉर्मेट है, जो प्रोजेक्ट की सेटिंग्स Prj::DurationFormat में परिभाषित है। |
| [GetPageCount (7 overloads)](./getpagecount/) | डिफ़ॉल्ट Timescale (Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पृष्ठ गणना लौटाता है। |
| [GetPredecessors](./getpredecessors/) | निर्दिष्ट कार्य के पूर्वज होने वाले टास्क लिंक का संग्रह लौटाता है। |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | स्ट्रीम से प्रोजेक्ट फ़ाइल जानकारी प्राप्त करता है। |
| [GetWork](./getwork/) | निर्दिष्ट डबल मान और डिफ़ॉल्ट कार्य फ़ॉर्मेट के साथ Duration ऑब्जेक्ट प्राप्त करता है। |
| [Recalculate (2 overloads)](./recalculate/) | सभी प्रोजेक्ट टास्क आईडी, आउटलाइन लेवल, शुरू/समाप्ति तिथियों को पुनः निर्धारित करता है, प्रारंभिक/अंतिम तिथियों को सेट करता है, स्लैक, कार्य और लागत फ़ील्ड की गणना करता है। |
| [RecalculateResourceFields](./recalculateresourcefields/) | संसाधनों के Id, प्रारंभ और समाप्ति को पुनः गणना करता है। |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | संसाधनों के प्रारंभ और समाप्ति को पुनः गणना करता है। |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | प्रोजेक्ट संसाधन असाइनमेंट सूची से अमान्य संसाधन असाइनमेंट को हटाता है। |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | सभी टास्क के WBS कोड को पुनः क्रमांकित करता है। |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | निर्दिष्ट तिथि के बाद शुरू होने के लिए अपूर्ण प्रोजेक्ट कार्य को पुनः निर्धारित करता है। |
| [Save (5 overloads)](./save/) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके प्रोजेक्ट को स्ट्रीम में सहेजता है। |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | प्रोजेक्ट को टेम्पलेट के रूप में निर्दिष्ट स्ट्रीम में सहेजता है। |
| [SaveReport (4 overloads)](./savereport/) | प्रोजेक्ट ओवरव्यू रिपोर्ट को स्ट्रीम में सहेजता है। |
| [SelectAllChildTasks](./selectallchildtasks/) | रूट टास्क के सभी चाइल्ड टास्क को पुनरावर्ती रूप से एकत्र करता है। |
| [Set (2 overloads)](./set/) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान से मैप करता है। |
| [set_ActualsInSync](./set_actualsinsync/) | ActualsInSync सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_AdminProject](./set_adminproject/) | AdminProject सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | AreEditableActualCosts सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_Author](./set_author/) | Author का मान सेट करता है। |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | AutoAddNewResourcesAndTasks सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | असाइनमेंट की कार्य और संसाधन दरों का उपयोग करके असाइनमेंट लागत और शेष लागत को स्वतः गणना किया जाना चाहिए या नहीं, यह सेट करता है। |
| [set_Autolink](./set_autolink/) | Autolink सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | BaselineForEarnedValue का मान सेट करता है। |
| [set_CalculationMode](./set_calculationmode/) | प्रोजेक्ट की गणना मोड सेट करता है। यह CalculationMode एनेमरेशन के मानों में से एक हो सकता है। |
| [set_Calendar](./set_calendar/) | Calendar का मान सेट करता है। |
| [set_Category](./set_category/) | Category का मान सेट करता है। |
| [set_Comments](./set_comments/) | Comments का मान सेट करता है। |
| [set_Company](./set_company/) | Company का मान सेट करता है। |
| [set_CreationDate](./set_creationdate/) | CreationDate का मान सेट करता है। |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | CriticalSlackLimit का मान सेट करता है। |
| [set_CurrencyCode](./set_currencycode/) | CurrencyCode का मान सेट करता है। |
| [set_CurrencyDigits](./set_currencydigits/) | CurrencyDigits का मान सेट करता है। |
| [set_CurrencySymbol](./set_currencysymbol/) | CurrencySymbol का मान सेट करता है। |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | CurrencySymbolPosition का मान सेट करता है। |
| [set_CurrentDate](./set_currentdate/) | CurrentDate का मान सेट करता है। |
| [set_CustomDateFormat](./set_customdateformat/) | CustomDateFormat का मान सेट करता है। |
| [set_DateFormat](./set_dateformat/) | DateFormat का मान सेट करता है। |
| [set_DaysPerMonth](./set_dayspermonth/) | DaysPerMonth का मान सेट करता है। |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | DefaultFinishTime का मान सेट करता है। |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | DefaultFixedCostAccrual का मान सेट करता है। |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | DefaultOvertimeRate का मान सेट करता है। |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | DefaultStandardRate का मान सेट करता है। |
| [set_DefaultStartTime](./set_defaultstarttime/) | DefaultStartTime का मान सेट करता है। |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | DefaultTaskEVMethod का मान सेट करता है। |
| [set_DefaultTaskType](./set_defaulttasktype/) | DefaultTaskType का मान सेट करता है। |
| [set_DefaultView](./set_defaultview/) | परियोजना का डिफ़ॉल्ट दृश्य सेट करता है। |
| [set_DurationFormat](./set_durationformat/) | DurationFormat का मान सेट करता है। |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod का मान सेट करता है। |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | ExtendedCreationDate का मान सेट करता है। |
| [set_FinishDate](./set_finishdate/) | FinishDate का मान सेट करता है। |
| [set_FiscalYearStart](./set_fiscalyearstart/) | FiscalYearStart सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_FyStartDate](./set_fystartdate/) | FyStartDate का मान सेट करता है। |
| [set_Guid](./set_guid/) | GUID का मान सेट करता है। |
| [set_HonorConstraints](./set_honorconstraints/) | HonorConstraints सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_HyperlinkBase](./set_hyperlinkbase/) | HyperlinkBase का मान सेट करता है। |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | InsertedProjectsLikeSummary सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_Keywords](./set_keywords/) | Keywords का मान सेट करता है। |
| [set_LastAuthor](./set_lastauthor/) | LastAuthor का मान सेट करता है। |
| [set_LastPrinted](./set_lastprinted/) | LastPrinted का मान सेट करता है। |
| [set_LastSaved](./set_lastsaved/) | LastSaved का मान सेट करता है। |
| [set_Manager](./set_manager/) | Manager का मान सेट करता है। |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | MicrosoftProjectServerURL सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_MinutesPerDay](./set_minutesperday/) | MinutesPerDay का मान सेट करता है। |
| [set_MinutesPerWeek](./set_minutesperweek/) | MinutesPerWeek का मान सेट करता है। |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | MoveCompletedEndsBack सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | MoveCompletedEndsForward सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | MoveRemainingStartsBack सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | एक मान सेट करता है जो दर्शाता है कि MoveRemainingStartsForward सेट है या नहीं। |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | एक मान सेट करता है जो दर्शाता है कि MultipleCriticalPaths सेट है या नहीं। |
| [set_Name](./set_name/) | Name का मान सेट करता है। |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | एक मान सेट करता है जो दर्शाता है कि NewTasksAreManual सेट है या नहीं। |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | एक मान सेट करता है जो दर्शाता है कि NewTasksEffortDriven सेट है या नहीं। |
| [set_NewTasksEstimated](./set_newtasksestimated/) | एक मान सेट करता है जो दर्शाता है कि NewTasksEstimated सेट है या नहीं। |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | NewTaskStartDate का मान सेट करता है। |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | एक मान सेट करता है जो दर्शाता है कि ProjectExternallyEdited सेट है या नहीं। |
| [set_RemoveFileProperties](./set_removefileproperties/) | एक मान सेट करता है जो दर्शाता है कि RemoveFileProperties सेट है या नहीं। |
| [set_Revision](./set_revision/) | Revision का मान सेट करता है। |
| [set_SaveVersion](./set_saveversion/) | SaveVersion का मान सेट करता है। |
| [set_ScheduleFromStart](./set_schedulefromstart/) | एक मान सेट करता है जो दर्शाता है कि ScheduleFromStart सेट है या नहीं। |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | एक मान सेट करता है जो दर्शाता है कि ShowProjectSummaryTask सेट है या नहीं। |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | एक मान सेट करता है जो दर्शाता है कि SplitsInProgressTasks सेट है या नहीं। |
| [set_SpreadActualCost](./set_spreadactualcost/) | एक मान सेट करता है जो दर्शाता है कि SpreadActualCost सेट है या नहीं। |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | एक मान सेट करता है जो दर्शाता है कि SpreadPercentComplete सेट है या नहीं। |
| [set_StartDate](./set_startdate/) | StartDate का मान सेट करता है। |
| [set_StatusDate](./set_statusdate/) | StatusDate का मान सेट करता है। |
| [set_Subject](./set_subject/) | Subject का मान सेट करता है। |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | एक मान सेट करता है जो दर्शाता है कि TaskUpdatesResource सेट है या नहीं। |
| [set_Template](./set_template/) | Template का मान सेट करता है। |
| [set_TimescaleFinish](./set_timescalefinish/) | TimescaleFinish का मान सेट करता है। |
| [set_TimescaleStart](./set_timescalestart/) | TimescaleStart का मान सेट करता है। |
| [set_Title](./set_title/) | Title का मान सेट करता है। |
| [set_Uid](./set_uid/) | Uid का मान सेट करता है। |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | एक मान सेट करता है जो दर्शाता है कि UpdateManuallyScheduledTasksWhenEditingLinks सेट है या नहीं। |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | परियोजना के लिए WBS कोड परिभाषा सेट करता है। |
| [set_WeekStartDay](./set_weekstartday/) | WeekStartDay का मान सेट करता है। |
| [set_WorkFormat](./set_workformat/) | WorkFormat का मान सेट करता है। |
| [SetBaseline (2 overloads)](./setbaseline/) | पूरे प्रोजेक्ट के लिए निर्दिष्ट बेसलाइन में बेसलाइन फ़ील्ड सहेजता है। |
| [SetBaselineSaveTime](./setbaselinesavetime/) | बेसलाइन सहेजने का समय सेट करता है। |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | पूरे प्रोजेक्ट के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है। |

