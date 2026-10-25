---
title: "Aspose::Tasks::Task क्लास"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks C++ के लिए"
description: "प्रोजेक्ट में एक कार्य का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

प्रोजेक्ट में एक कार्य का प्रतिनिधित्व करता है।

Task एक एकल परम कार्य खंड का प्रतिनिधित्व करता है।

एक व्यक्ति Task का उपयोग करके प्रोजेक्ट की योजना बना सकता है, कार्य बनाकर और उपयुक्त संसाधनों को उन पर असाइन करके। प्रोजेक्ट में कार्य एक मूल पदानुक्रमित वृक्ष संरचना के रूप में व्यवस्थित होते हैं, जिसमें एक रूट टास्क और बच्चों के कार्यों की उपवृक्षें होती हैं।

टास्क की ट्री बनाने के लिए आप Aspose::Tasks::TaskCollection नामक एक विशेष संग्रह का उपयोग कर सकते हैं, Project::RootTask प्रॉपर्टी तक पहुंचकर, उदाहरण के लिए:

```cpp
Project project = new Project();
 
// नए टास्क जोड़ें
Task task1 = project.RootTask.Children.Add(); // a parent task with empty name is added
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserts a task before the childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));
 
// प्रोजेक्ट को उपलब्ध फ़ॉर्मैट्स में से किसी एक में सहेजें
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Clone](./clone/) | सबटास्क के बिना टास्क की पूरी कॉपी बनाता है। |
| [Delete](./delete/) | पैरेंट प्रोजेक्ट टास्क संग्रह से टास्क और उसकी सभी असाइनमेंट्स को हटाता है। |
| [Equals (2 overloads)](./equals/) | वापस देता है एक मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [Get](./get/) | इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है। |
| [get_ActivityId](./get_activityid/) | activity id फ़ील्ड का प्रतिनिधित्व करता है - Primavera द्वारा उपयोग किया गया कार्य का अद्वितीय पहचानकर्ता। (केवल Primavera प्रोजेक्ट्स पर लागू)। |
| [get_ActualCost](./get_actualcost/) | ActualCost का मान प्राप्त करता है। |
| [get_ActualDuration](./get_actualduration/) | ActualDuration का मान प्राप्त करता है। |
| [get_ActualFinish](./get_actualfinish/) | ActualFinish का मान प्राप्त करता है। |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | एक मान प्राप्त करता है ActualOvertimeCost। |
| [get_ActualOvertimeWork](./get_actualovertimework/) | एक मान प्राप्त करता है ActualOvertimeWork। |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | एक मान प्राप्त करता है ActualOvertimeWorkProtected। |
| [get_ActualStart](./get_actualstart/) | ActualStart का मान प्राप्त करता है। |
| [get_ActualWork](./get_actualwork/) | एक मान प्राप्त करता है ActualWork। |
| [get_ActualWorkProtected](./get_actualworkprotected/) | एक मान प्राप्त करता है ActualWorkProtected। |
| [get_ACWP](./get_acwp/) | एक मान प्राप्त करता है ACWP। |
| [get_Assignments](./get_assignments/) | इस वस्तु के लिए संसाधन असाइनमेंट का संग्रह प्राप्त करता है। |
| [get_Baselines](./get_baselines/) | टास्क के बेसलाइन मानों का संग्रह प्राप्त करता है। |
| [get_BCWP](./get_bcwp/) | एक मान प्राप्त करता है BCWP। |
| [get_BCWS](./get_bcws/) | एक मान प्राप्त करता है BCWS। |
| [get_BudgetCost](./get_budgetcost/) | एक मान प्राप्त करता है BudgetCost। |
| [get_BudgetWork](./get_budgetwork/) | एक मान प्राप्त करता है BudgetWork। |
| [get_Calendar](./get_calendar/) | एक मान प्राप्त करता है Calendar। |
| [get_Children](./get_children/) | इस ऑब्जेक्ट का चाइल्ड टास्क संग्रह प्राप्त करता है। TaskCollection ऑब्जेक्ट जो चाइल्ड टास्क को दर्शाता है। |
| [get_CommitmentFinish](./get_commitmentfinish/) | CommitmentFinish का मान प्राप्त करता है। |
| [get_CommitmentStart](./get_commitmentstart/) | CommitmentStart का मान प्राप्त करता है। |
| [get_CommitmentType](./get_commitmenttype/) | CommitmentType का मान प्राप्त करता है। |
| [get_ConstraintDate](./get_constraintdate/) | ConstraintDate का मान प्राप्त करता है। |
| [get_ConstraintType](./get_constrainttype/) | ConstraintType का मान प्राप्त करता है। |
| [get_Contact](./get_contact/) | Contact का मान प्राप्त करता है। |
| [get_Cost](./get_cost/) | एक मान प्राप्त करता है Cost। |
| [get_CostVariance](./get_costvariance/) | एक मान प्राप्त करता है CostVariance। |
| [get_Created](./get_created/) | Created का मान प्राप्त करता है। |
| [get_CV](./get_cv/) | CV का मान प्राप्त करता है। |
| [get_Deadline](./get_deadline/) | Deadline का मान प्राप्त करता है। |
| [get_DisplayAsSummary](./get_displayassummary/) | यह दर्शाता है कि DisplayAsSummary सेट है या नहीं, इसका मान प्राप्त करता है। |
| [get_DisplayOnTimeline](./get_displayontimeline/) | यह दर्शाता है कि DisplayOnTimeline सेट है या नहीं, इसका मान प्राप्त करता है। |
| [get_Duration](./get_duration/) | Duration का मान प्राप्त करता है। |
| [get_DurationFormat](./get_durationformat/) | DurationFormat का मान प्राप्त करता है। |
| [get_DurationText](./get_durationtext/) | DurationText का मान प्राप्त करता है। |
| [get_DurationVariance](./get_durationvariance/) | DurationVariance का मान प्राप्त करता है। |
| [get_EarlyFinish](./get_earlyfinish/) | EarlyFinish का मान प्राप्त करता है। |
| [get_EarlyStart](./get_earlystart/) | EarlyStart का मान प्राप्त करता है। |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | EarnedValueMethod का मान प्राप्त करता है। |
| [get_ExtendedAttributes](./get_extendedattributes/) | ExtendedAttributeCollection ऑब्जेक्ट प्राप्त करता है जिसमें विस्तारित एट्रिब्यूट के मान होते हैं। |
| [get_ExternalId](./get_externalid/) | ExternalId का मान प्राप्त करता है। |
| [get_ExternalTaskProject](./get_externaltaskproject/) | ExternalTaskProject का मान प्राप्त करता है। |
| [get_ExternalUid](./get_externaluid/) | बाहरी कार्य के बाहरी होने पर उसका अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है। |
| [get_Finish](./get_finish/) | Finish का मान प्राप्त करता है। |
| [get_FinishSlack](./get_finishslack/) | FinishSlack का मान प्राप्त करता है। |
| [get_FinishText](./get_finishtext/) | FinishText का मान प्राप्त करता है। |
| [get_FinishVariance](./get_finishvariance/) | FinishVariance का मान प्राप्त करता है। |
| [get_FixedCost](./get_fixedcost/) | FixedCost का मान प्राप्त करता है। |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | FixedCostAccrual का मान प्राप्त करता है। |
| [get_FreeSlack](./get_freeslack/) | FreeSlack का मान प्राप्त करता है। |
| [get_Guid](./get_guid/) | Guid का मान प्राप्त करता है। |
| [get_HideBar](./get_hidebar/) | HideBar सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_Hyperlink](./get_hyperlink/) | कार्य से जुड़ी हाइपरलिंक के लिए शीर्षक या व्याख्यात्मक पाठ प्राप्त करता है। |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | कार्य से जुड़ी हाइपरलिंक का पता प्राप्त करता है। |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | कार्य से जुड़ी हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को प्राप्त करता है। |
| [get_Id](./get_id/) | Id का मान प्राप्त करता है। |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | IgnoreResourceCalendar सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IgnoreWarnings](./get_ignorewarnings/) | IgnoreWarnings सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsActive](./get_isactive/) | IsActive सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsCritical](./get_iscritical/) | IsCritical सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsEffortDriven](./get_iseffortdriven/) | IsEffortDriven सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsEstimated](./get_isestimated/) | IsEstimated सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsExpanded](./get_isexpanded/) | IsExpanded सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsExternalTask](./get_isexternaltask/) | IsExternalTask सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsManual](./get_ismanual/) | IsManual सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsMarked](./get_ismarked/) | IsMarked सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsMilestone](./get_ismilestone/) | IsMilestone सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsNull](./get_isnull/) | यह संकेत करने वाला मान प्राप्त करता है कि IsNull सेट है या नहीं। |
| [get_IsOverallocated](./get_isoverallocated/) | IsOverallocated सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsPublished](./get_ispublished/) | IsPublished सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsRecurring](./get_isrecurring/) | IsRecurring सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsResumeValid](./get_isresumevalid/) | IsResumeValid सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [get_IsRollup](./get_isrollup/) | एक मान प्राप्त करता है जो दर्शाता है कि IsRollup सेट है या नहीं। |
| [get_IsSubproject](./get_issubproject/) | एक मान प्राप्त करता है जो दर्शाता है कि IsSubproject सेट है या नहीं। |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | एक मान प्राप्त करता है जो दर्शाता है कि IsSubprojectReadOnly सेट है या नहीं। |
| [get_IsSummary](./get_issummary/) | एक मान प्राप्त करता है जो दर्शाता है कि IsSummary सेट है या नहीं। |
| [get_LateFinish](./get_latefinish/) | LateFinish का मान प्राप्त करता है। |
| [get_LateStart](./get_latestart/) | LateStart का मान प्राप्त करता है। |
| [get_LevelAssignments](./get_levelassignments/) | एक मान प्राप्त करता है जो दर्शाता है कि LevelAssignments सेट है या नहीं। |
| [get_LevelingCanSplit](./get_levelingcansplit/) | एक मान प्राप्त करता है जो दर्शाता है कि LevelingCanSplit सेट है या नहीं। |
| [get_LevelingDelay](./get_levelingdelay/) | LevelingDelay का मान प्राप्त करता है। |
| [get_ManualDuration](./get_manualduration/) | ManualDuration का मान प्राप्त करता है। |
| [get_ManualFinish](./get_manualfinish/) | ManualFinish का मान प्राप्त करता है। |
| [get_ManualStart](./get_manualstart/) | ManualStart का मान प्राप्त करता है। |
| [get_Name](./get_name/) | Name का मान प्राप्त करता है। |
| [get_NotesRTF](./get_notesrtf/) | NotesRTF का मान प्राप्त करता है। |
| [get_NotesText](./get_notestext/) | NotesText का मान प्राप्त करता है। |
| [get_OutlineCodes](./get_outlinecodes/) | OutlineCodeCollection ऑब्जेक्ट प्राप्त करता है। |
| [get_OutlineLevel](./get_outlinelevel/) | OutlineLevel का मान प्राप्त करता है। |
| [get_OutlineNumber](./get_outlinenumber/) | OutlineNumber का मान प्राप्त करता है। |
| [get_OvertimeCost](./get_overtimecost/) | OvertimeCost का मान प्राप्त करता है। |
| [get_OvertimeWork](./get_overtimework/) | OvertimeWork का मान प्राप्त करता है। |
| [get_ParentProject](./get_parentproject/) | एक कार्य का पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [get_ParentTask](./get_parenttask/) | एक कार्य का पैरेंट टास्क प्राप्त करता है। |
| [get_PercentComplete](./get_percentcomplete/) | PercentComplete का मान प्राप्त करता है। |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | PercentWorkComplete का मान प्राप्त करता है। |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | PhysicalPercentComplete का मान प्राप्त करता है। |
| [get_Predecessors](./get_predecessors/) | एक TaskCollection ऑब्जेक्ट प्राप्त करता है जिसमें इस Task ऑब्जेक्ट के सभी प्रीडेसर्स शामिल होते हैं। |
| [get_PreleveledFinish](./get_preleveledfinish/) | PreleveledFinish का मान प्राप्त करता है। |
| [get_PreleveledStart](./get_preleveledstart/) | PreleveledStart का मान प्राप्त करता है। |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Primavera फ़ाइल से पढ़े गए एक कार्य के लिए Primavera-विशिष्ट प्रॉपर्टीज़ वाला ऑब्जेक्ट प्राप्त करता है। |
| [get_Priority](./get_priority/) | Priority का मान प्राप्त करता है। |
| [get_RecurringInfo](./get_recurringinfo/) | एक पुनरावर्ती कार्य के लिए RecurringTaskInfo क्लास का इंस्टेंस प्राप्त करता है; यदि कार्य पुनरावर्ती नहीं है तो null लौटाता है; |
| [get_RegularWork](./get_regularwork/) | RegularWork का मान प्राप्त करता है। |
| [get_RemainingCost](./get_remainingcost/) | RemainingCost का मान प्राप्त करता है। |
| [get_RemainingDuration](./get_remainingduration/) | RemainingDuration का मान प्राप्त करता है। |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | RemainingOvertimeCost का मान प्राप्त करता है। |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | RemainingOvertimeWork का मान प्राप्त करता है। |
| [get_RemainingWork](./get_remainingwork/) | RemainingWork का मान प्राप्त करता है। |
| [get_Resume](./get_resume/) | Resume का मान प्राप्त करता है। |
| [get_SplitParts](./get_splitparts/) | एक SplitPart संग्रह प्राप्त करता है जो कार्य के भागों का प्रतिनिधित्व करता है। |
| [get_Start](./get_start/) | Start का मान प्राप्त करता है। |
| [get_StartSlack](./get_startslack/) | StartSlack का मान प्राप्त करता है। |
| [get_StartText](./get_starttext/) | StartText का मान प्राप्त करता है। |
| [get_StartVariance](./get_startvariance/) | StartVariance का मान प्राप्त करता है। |
| [get_Status](./get_status/) | कार्य की स्थिति प्राप्त करता है। |
| [get_StatusManager](./get_statusmanager/) | StatusManager का मान प्राप्त करता है। |
| [get_Stop](./get_stop/) | Stop का मान प्राप्त करता है। |
| [get_SubprojectName](./get_subprojectname/) | SubprojectName का मान प्राप्त करता है। |
| [get_Successors](./get_successors/) | एक TaskCollection ऑब्जेक्ट प्राप्त करता है जिसमें इस Task ऑब्जेक्ट के सभी उत्तराधिकारी शामिल होते हैं। |
| [get_SV](./get_sv/) | अर्जित मूल्य अनुसूची विचलन, प्रोजेक्ट स्थिति तिथि तक। अनुसूची विचलन (SV) BCWP और BCWS के बीच का अंतर है। |
| [get_TimephasedData](./get_timephaseddata/) | इस कार्य का एक TimephasedDataCollection ऑब्जेक्ट प्राप्त करता है। कार्य से जुड़ा समय-फ़ेज़्ड डेटा ब्लॉक। |
| [get_TotalSlack](./get_totalslack/) | TotalSlack का मान प्राप्त करता है। |
| [get_Type](./get_type/) | Type का मान प्राप्त करता है। |
| [get_Uid](./get_uid/) | Uid का मान प्राप्त करता है। |
| [get_Warning](./get_warning/) | एक मान प्राप्त करता है जो दर्शाता है कि Warning सेट है या नहीं। |
| [get_WBS](./get_wbs/) | WBS का मान प्राप्त करता है। |
| [get_WBSLevel](./get_wbslevel/) | WBSLevel का मान प्राप्त करता है। |
| [get_Work](./get_work/) | Work का मान प्राप्त करता है। |
| [get_WorkVariance](./get_workvariance/) | WorkVariance का मान प्राप्त करता है। |
| [GetHashCode](./gethashcode/) | इस Task के लिए एक हैश कोड मान लौटाता है। |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | दिए गए प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData मानों के साथ TimephasedDataCollection ऑब्जेक्ट लौटाता है। |
| [MoveToSibling (2 overloads)](./movetosibling/) | वर्तमान कार्य को उसी Outline Level पर निर्दिष्ट कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को बुलाना चाहिए (यह सभी प्रोजेक्ट कार्यों को (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करता है) पुनः समय-सारिणी करेगा और स्लैक, कार्य और लागत फ़ील्ड जैसे निर्भर फ़ील्ड की गणना करेगा, outline levels)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य आईडी, outline level और outline numbers को स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः समय-सारिणी करेगी (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करती है, स्लैक, कार्य और लागत फ़ील्ड की गणना करती है, आईडी और outline levels को पुनः गणना करती है)। |
| [OutlineIndent](./outlineindent/) | आउटलाइन में एक कार्य को इंडेंट करता है। |
| [OutlineOutdent](./outlineoutdent/) | आउटलाइन में एक कार्य को प्रोमोट करता है। |
| [SelectAllChildTasks](./selectallchildtasks/) | इस कार्य के सभी चाइल्ड टास्क को पुनरावर्ती रूप से एकत्र करता है। |
| [Set](./set/) | इस कंटेनर में निर्दिष्ट प्रॉपर्टी को निर्दिष्ट मान से मैप करता है। |
| [set_ActivityId](./set_activityid/) | activity id फ़ील्ड का प्रतिनिधित्व करता है - Primavera द्वारा उपयोग किया गया कार्य का अद्वितीय पहचानकर्ता। (केवल Primavera प्रोजेक्ट्स पर लागू)। |
| [set_ActualCost](./set_actualcost/) | ActualCost का मान सेट करता है। |
| [set_ActualDuration](./set_actualduration/) | ActualDuration का मान सेट करता है। |
| [set_ActualFinish](./set_actualfinish/) | ActualFinish का मान सेट करता है। |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | ActualOvertimeCost का मान सेट करता है। |
| [set_ActualOvertimeWork](./set_actualovertimework/) | ActualOvertimeWork का मान सेट करता है। |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | ActualOvertimeWorkProtected का मान सेट करता है। |
| [set_ActualStart](./set_actualstart/) | ActualStart का मान सेट करता है। |
| [set_ActualWork](./set_actualwork/) | ActualWork का मान सेट करता है। |
| [set_ActualWorkProtected](./set_actualworkprotected/) | ActualWorkProtected का मान सेट करता है। |
| [set_ACWP](./set_acwp/) | ACWP का मान सेट करता है। |
| [set_Baselines](./set_baselines/) | कार्य के बेसलाइन मानों का संग्रह सेट करता है। |
| [set_BCWP](./set_bcwp/) | BCWP का मान सेट करता है। |
| [set_BCWS](./set_bcws/) | BCWS का मान सेट करता है। |
| [set_BudgetCost](./set_budgetcost/) | BudgetCost का मान सेट करता है। |
| [set_BudgetWork](./set_budgetwork/) | BudgetWork का मान सेट करता है। |
| [set_Calendar](./set_calendar/) | Calendar का मान सेट करता है। |
| [set_CommitmentFinish](./set_commitmentfinish/) | CommitmentFinish का मान सेट करता है। |
| [set_CommitmentStart](./set_commitmentstart/) | CommitmentStart का मान सेट करता है। |
| [set_CommitmentType](./set_commitmenttype/) | CommitmentType का मान सेट करता है। |
| [set_ConstraintDate](./set_constraintdate/) | ConstraintDate का मान सेट करता है। |
| [set_ConstraintType](./set_constrainttype/) | ConstraintType का मान सेट करता है। |
| [set_Contact](./set_contact/) | संपर्क का मान सेट करता है। |
| [set_Cost](./set_cost/) | कॉस्ट का मान सेट करता है। |
| [set_CostVariance](./set_costvariance/) | कॉस्टवेरिएंस का मान सेट करता है। |
| [set_Created](./set_created/) | क्रिएटेड का मान सेट करता है। |
| [set_CV](./set_cv/) | CV का मान सेट करता है। |
| [set_Deadline](./set_deadline/) | समयसीमा का मान सेट करता है। |
| [set_DisplayAsSummary](./set_displayassummary/) | यह दर्शाता है कि DisplayAsSummary सेट है या नहीं, इसका मान सेट करता है। |
| [set_DisplayOnTimeline](./set_displayontimeline/) | यह दर्शाता है कि DisplayOnTimeline सेट है या नहीं, इसका मान सेट करता है। |
| [set_Duration](./set_duration/) | अवधि का मान सेट करता है। |
| [set_DurationFormat](./set_durationformat/) | DurationFormat का मान सेट करता है। |
| [set_DurationText](./set_durationtext/) | DurationText का मान सेट करता है। |
| [set_DurationVariance](./set_durationvariance/) | DurationVariance का मान सेट करता है। |
| [set_EarlyFinish](./set_earlyfinish/) | EarlyFinish का मान सेट करता है। |
| [set_EarlyStart](./set_earlystart/) | EarlyStart का मान सेट करता है। |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | EarnedValueMethod का मान सेट करता है। |
| [set_ExternalId](./set_externalid/) | ExternalId का मान सेट करता है। |
| [set_ExternalTaskProject](./set_externaltaskproject/) | ExternalTaskProject का मान सेट करता है। |
| [set_ExternalUid](./set_externaluid/) | बाहरी कार्य के बाहरी होने पर उसका अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है। |
| [set_Finish](./set_finish/) | फ़िनिश का मान सेट करता है। |
| [set_FinishSlack](./set_finishslack/) | FinishSlack का मान सेट करता है। |
| [set_FinishText](./set_finishtext/) | FinishText का मान सेट करता है। |
| [set_FinishVariance](./set_finishvariance/) | FinishVariance का मान सेट करता है। |
| [set_FixedCost](./set_fixedcost/) | FixedCost का मान सेट करता है। |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | FixedCostAccrual का मान सेट करता है। |
| [set_FreeSlack](./set_freeslack/) | FreeSlack का मान सेट करता है। |
| [set_Guid](./set_guid/) | GUID का मान सेट करता है। |
| [set_HideBar](./set_hidebar/) | यह दर्शाता है कि HideBar सेट है या नहीं, इसका मान सेट करता है। |
| [set_Hyperlink](./set_hyperlink/) | कार्य से जुड़े हाइपरलिंक के लिए शीर्षक या व्याख्यात्मक पाठ सेट करता है। |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | कार्य से जुड़े हाइपरलिंक का पता सेट करता है। |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | कार्य से जुड़े हाइपरलिंक में दस्तावेज़ के विशिष्ट स्थान को सेट करता है। |
| [set_Id](./set_id/) | आईडी का मान सेट करता है। |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | यह दर्शाता है कि IgnoreResourceCalendar सेट है या नहीं, इसका मान सेट करता है। |
| [set_IgnoreWarnings](./set_ignorewarnings/) | यह दर्शाता है कि IgnoreWarnings सेट है या नहीं, इसका मान सेट करता है। |
| [set_IsActive](./set_isactive/) | यह दर्शाता है कि IsActive सेट है या नहीं, इसका मान सेट करता है। |
| [set_IsCritical](./set_iscritical/) | यह दर्शाता है कि IsCritical सेट है या नहीं, इसका मान सेट करता है। |
| [set_IsEffortDriven](./set_iseffortdriven/) | यह दर्शाता है कि IsEffortDriven सेट है या नहीं, इसका मान सेट करता है। |
| [set_IsEstimated](./set_isestimated/) | एक मान सेट करता है जो इंगित करता है कि IsEstimated सेट है या नहीं। |
| [set_IsExpanded](./set_isexpanded/) | एक मान सेट करता है जो इंगित करता है कि IsExpanded सेट है या नहीं। |
| [set_IsExternalTask](./set_isexternaltask/) | एक मान सेट करता है जो इंगित करता है कि IsExternalTask सेट है या नहीं। |
| [set_IsManual](./set_ismanual/) | एक मान सेट करता है जो इंगित करता है कि IsManual सेट है या नहीं। |
| [set_IsMarked](./set_ismarked/) | एक मान सेट करता है जो इंगित करता है कि IsMarked सेट है या नहीं। |
| [set_IsMilestone](./set_ismilestone/) | एक मान सेट करता है जो इंगित करता है कि IsMilestone सेट है या नहीं। |
| [set_IsNull](./set_isnull/) | यह संकेत करने वाला मान सेट करता है कि IsNull सेट है या नहीं। |
| [set_IsOverallocated](./set_isoverallocated/) | एक मान सेट करता है जो इंगित करता है कि IsOverallocated सेट है या नहीं। |
| [set_IsPublished](./set_ispublished/) | एक मान सेट करता है जो इंगित करता है कि IsPublished सेट है या नहीं। |
| [set_IsRecurring](./set_isrecurring/) | एक मान सेट करता है जो इंगित करता है कि IsRecurring सेट है या नहीं। |
| [set_IsResumeValid](./set_isresumevalid/) | एक मान सेट करता है जो इंगित करता है कि IsResumeValid सेट है या नहीं। |
| [set_IsRollup](./set_isrollup/) | एक मान सेट करता है जो इंगित करता है कि IsRollup सेट है या नहीं। |
| [set_IsSubproject](./set_issubproject/) | एक मान सेट करता है जो इंगित करता है कि IsSubproject सेट है या नहीं। |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | एक मान सेट करता है जो इंगित करता है कि IsSubprojectReadOnly सेट है या नहीं। |
| [set_IsSummary](./set_issummary/) | एक मान सेट करता है जो इंगित करता है कि IsSummary सेट है या नहीं। |
| [set_LateFinish](./set_latefinish/) | LateFinish का मान सेट करता है। |
| [set_LateStart](./set_latestart/) | LateStart का मान सेट करता है। |
| [set_LevelAssignments](./set_levelassignments/) | एक मान सेट करता है जो इंगित करता है कि LevelAssignments सेट है या नहीं। |
| [set_LevelingCanSplit](./set_levelingcansplit/) | एक मान सेट करता है जो इंगित करता है कि LevelingCanSplit सेट है या नहीं। |
| [set_LevelingDelay](./set_levelingdelay/) | LevelingDelay का मान सेट करता है। |
| [set_ManualDuration](./set_manualduration/) | ManualDuration का मान सेट करता है। |
| [set_ManualFinish](./set_manualfinish/) | ManualFinish का मान सेट करता है। |
| [set_ManualStart](./set_manualstart/) | ManualStart का मान सेट करता है। |
| [set_Name](./set_name/) | Name का मान सेट करता है। |
| [set_NotesRTF](./set_notesrtf/) | NotesRTF का मान सेट करता है। |
| [set_NotesText](./set_notestext/) | NotesText का मान सेट करता है। |
| [set_OutlineCodes](./set_outlinecodes/) | OutlineCodeCollection ऑब्जेक्ट सेट करता है। |
| [set_OutlineLevel](./set_outlinelevel/) | OutlineLevel का मान सेट करता है। |
| [set_OutlineNumber](./set_outlinenumber/) | OutlineNumber का मान सेट करता है। |
| [set_OvertimeCost](./set_overtimecost/) | OvertimeCost का मान सेट करता है। |
| [set_OvertimeWork](./set_overtimework/) | OvertimeWork का मान सेट करता है। |
| [set_PercentComplete](./set_percentcomplete/) | PercentComplete का मान सेट करता है। |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | PercentWorkComplete का मान सेट करता है। |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | PhysicalPercentComplete का मान सेट करता है। |
| [set_PreleveledFinish](./set_preleveledfinish/) | PreleveledFinish का मान सेट करता है। |
| [set_PreleveledStart](./set_preleveledstart/) | PreleveledStart का मान सेट करता है। |
| [set_Priority](./set_priority/) | Priority का मान सेट करता है। |
| [set_RegularWork](./set_regularwork/) | RegularWork का मान सेट करता है। |
| [set_RemainingCost](./set_remainingcost/) | RemainingCost का मान सेट करता है। |
| [set_RemainingDuration](./set_remainingduration/) | RemainingDuration का मान सेट करता है। |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | RemainingOvertimeCost का मान सेट करता है। |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | RemainingOvertimeWork का मान सेट करता है। |
| [set_RemainingWork](./set_remainingwork/) | RemainingWork का मान सेट करता है। |
| [set_Resume](./set_resume/) | Resume का मान सेट करता है। |
| [set_Start](./set_start/) | Start का मान सेट करता है। |
| [set_StartSlack](./set_startslack/) | StartSlack का मान सेट करता है। |
| [set_StartText](./set_starttext/) | StartText का मान सेट करता है। |
| [set_StartVariance](./set_startvariance/) | StartVariance का मान सेट करता है। |
| [set_StatusManager](./set_statusmanager/) | StatusManager का मान सेट करता है। |
| [set_Stop](./set_stop/) | Stop का मान सेट करता है। |
| [set_SubprojectName](./set_subprojectname/) | SubprojectName का मान सेट करता है। |
| [set_SV](./set_sv/) | अर्जित मूल्य अनुसूची विचलन, प्रोजेक्ट स्थिति तिथि तक। अनुसूची विचलन (SV) BCWP और BCWS के बीच का अंतर है। |
| [set_TimephasedData](./set_timephaseddata/) | इस कार्य का TimephasedDataCollection ऑब्जेक्ट सेट करता है। कार्य से संबंधित समय‑फ़ेज़्ड डेटा ब्लॉक। |
| [set_TotalSlack](./set_totalslack/) | TotalSlack का मान सेट करता है। |
| [set_Type](./set_type/) | Type का मान सेट करता है। |
| [set_Uid](./set_uid/) | Uid का मान सेट करता है। |
| [set_Warning](./set_warning/) | Warning सेट है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [set_WBS](./set_wbs/) | WBS का मान सेट करता है। |
| [set_WBSLevel](./set_wbslevel/) | WBSLevel का मान सेट करता है। |
| [set_Work](./set_work/) | Work का मान सेट करता है। |
| [set_WorkVariance](./set_workvariance/) | WorkVariance का मान सेट करता है। |
| [ToString](./tostring/) | एक कार्य का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं। |

