---
title: Task
second_title: Aspose.Tasks for Java API Reference
description: Represents a task in a project.
type: docs
weight: 288
url: /java/com.aspose.tasks/task/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink, java.lang.Cloneable
```
public class Task extends IContainer<Byte> implements System.IEquatable<Task>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink, Cloneable
```

Represents a task in a project.

--------------------

The **Task** is representing a one atomic chunk of work.

One can use **Task** to plan a project by creating tasks and assign appropriate resources onto them. Tasks in a project are organized as a rooted hierarchical tree structure, with a root task and subtrees of children tasks.

To build a tree of tasks one can use a specialized collection [TaskCollection](../../com.aspose.tasks/taskcollection) by accessing `Project.RootTask`([Project.getRootTask](../../com.aspose.tasks/project\#getRootTask)/[Project.setRootTask(Task)](../../com.aspose.tasks/project\#setRootTask-Task-)) property e.g.:

```

``````

  Project project = new Project();
  // add new tasks
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

  // save project in the one of available formats
  project.Save("Filled project.xml", SaveFileFormat.Mpp);
  
```


## Methods

| Method | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returns the value to which the property is mapped in this container. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Maps the specified property to the specified value in this container. |
| [deepClone()](#deepClone--) | Creates full copy of a task without subtasks. |
| [delete()](#delete--) | Deletes a task from parent project tasks collection and all its assignments. |
| [equals(Task other)](#equals-com.aspose.tasks.Task-) | Returns a value indicating whether this instance is equal to a specified task. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getACWP()](#getACWP--) | Gets a value of ACWP. |
| [getActivityId()](#getActivityId--) | Represents activity id field - a task's unique identifier used by Primavera. |
| [getActualCost()](#getActualCost--) | Gets a value of ActualCost. |
| [getActualDuration()](#getActualDuration--) | Gets a value of ActualDuration. |
| [getActualFinish()](#getActualFinish--) | Gets a value of ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Gets a value of ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Gets a value of ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Gets a value of ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Gets a value of ActualStart. |
| [getActualWork()](#getActualWork--) | Gets a value of ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Gets a value of ActualWorkProtected. |
| [getAssignments()](#getAssignments--) | Gets a collection of resource assignments for this object. |
| [getBCWP()](#getBCWP--) | Gets a value of BCWP. |
| [getBCWS()](#getBCWS--) | Gets a value of BCWS. |
| [getBaselines()](#getBaselines--) | Gets the collection of baseline values of the task. |
| [getBudgetCost()](#getBudgetCost--) | Gets a value of BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Gets a value of BudgetWork. |
| [getCV()](#getCV--) | Gets a value of CV. |
| [getCalendar()](#getCalendar--) | Gets a value of Calendar. |
| [getChildren()](#getChildren--) | Gets a child task collection of this object. |
| [getCommitmentFinish()](#getCommitmentFinish--) | Gets a value of CommitmentFinish. |
| [getCommitmentStart()](#getCommitmentStart--) | Gets a value of CommitmentStart. |
| [getCommitmentType()](#getCommitmentType--) | Gets a value of CommitmentType. |
| [getConstraintDate()](#getConstraintDate--) | Gets a value of ConstraintDate. |
| [getConstraintType()](#getConstraintType--) | Gets a value of ConstraintType. |
| [getContact()](#getContact--) | Gets a value of Contact. |
| [getCost()](#getCost--) | Gets a value of Cost. |
| [getCostVariance()](#getCostVariance--) | Gets a value of CostVariance. |
| [getCreated()](#getCreated--) | Gets a value of Created. |
| [getDeadline()](#getDeadline--) | Gets a value of Deadline. |
| [getDisplayAsSummary()](#getDisplayAsSummary--) | Gets a value indicating whether DisplayAsSummary is set or not. |
| [getDisplayOnTimeline()](#getDisplayOnTimeline--) | Gets a value indicating whether DisplayOnTimeline is set or not. |
| [getDuration()](#getDuration--) | Gets a value of Duration. |
| [getDurationFormat()](#getDurationFormat--) | Gets a value of DurationFormat. |
| [getDurationText()](#getDurationText--) | Gets a value of DurationText. |
| [getDurationVariance()](#getDurationVariance--) | Gets a value of DurationVariance. |
| [getEarlyFinish()](#getEarlyFinish--) | Gets a value of EarlyFinish. |
| [getEarlyStart()](#getEarlyStart--) | Gets a value of EarlyStart. |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | Gets a value of EarnedValueMethod. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets ExtendedAttributeCollection object containing the values of an extended attribute. |
| [getExternalId()](#getExternalId--) | Gets a value of ExternalId. |
| [getExternalTaskProject()](#getExternalTaskProject--) | Gets a value of ExternalTaskProject. |
| [getExternalUid()](#getExternalUid--) | Gets the external task's Unique identifier when the task is external. |
| [getFinish()](#getFinish--) | Gets a value of Finish. |
| [getFinishSlack()](#getFinishSlack--) | Gets a value of FinishSlack. |
| [getFinishText()](#getFinishText--) | Gets a value of FinishText. |
| [getFinishVariance()](#getFinishVariance--) | Gets a value of FinishVariance. |
| [getFixedCost()](#getFixedCost--) | Gets a value of FixedCost. |
| [getFixedCostAccrual()](#getFixedCostAccrual--) | Gets a value of FixedCostAccrual. |
| [getFreeSlack()](#getFreeSlack--) | Gets a value of FreeSlack. |
| [getGuid()](#getGuid--) | Gets a value of Guid. |
| [getHideBar()](#getHideBar--) | Gets a value indicating whether HideBar is set or not. |
| [getHyperlink()](#getHyperlink--) | Gets the title or explanatory text for a hyperlink associated with a task. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Gets the address for a hyperlink associated with a task. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Gets the specific location in a document in a hyperlink associated with a task. |
| [getId()](#getId--) | Gets a value of Id. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Gets a value indicating whether IgnoreResourceCalendar is set or not. |
| [getIgnoreWarnings()](#getIgnoreWarnings--) | Gets a value indicating whether IgnoreWarnings is set or not. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLateFinish()](#getLateFinish--) | Gets a value of LateFinish. |
| [getLateStart()](#getLateStart--) | Gets a value of LateStart. |
| [getLevelAssignments()](#getLevelAssignments--) | Gets a value indicating whether LevelAssignments is set or not. |
| [getLevelingCanSplit()](#getLevelingCanSplit--) | Gets a value indicating whether LevelingCanSplit is set or not. |
| [getLevelingDelay()](#getLevelingDelay--) | Gets a value of LevelingDelay. |
| [getManualDuration()](#getManualDuration--) | Gets a value of ManualDuration. |
| [getManualFinish()](#getManualFinish--) | Gets a value of ManualFinish. |
| [getManualStart()](#getManualStart--) | Gets a value of ManualStart. |
| [getName()](#getName--) | Gets a value of Name. |
| [getNotesRTF()](#getNotesRTF--) | Gets a value of NotesRTF. |
| [getNotesText()](#getNotesText--) | Gets a value of NotesText. |
| [getOutlineCodes()](#getOutlineCodes--) | Gets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |
| [getOutlineLevel()](#getOutlineLevel--) | Gets a value of OutlineLevel. |
| [getOutlineNumber()](#getOutlineNumber--) | Gets a value of OutlineNumber. |
| [getOvertimeCost()](#getOvertimeCost--) | Gets a value of OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Gets a value of OvertimeWork. |
| [getParentProject()](#getParentProject--) | Gets the parent project of a task. |
| [getParentTask()](#getParentTask--) | Gets the parent task of a task. |
| [getPercentComplete()](#getPercentComplete--) | Gets a value of PercentComplete. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Gets a value of PercentWorkComplete. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Gets a value of PhysicalPercentComplete. |
| [getPredecessors()](#getPredecessors--) | Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all predecessors of this Task object. |
| [getPreleveledFinish()](#getPreleveledFinish--) | Gets a value of PreleveledFinish. |
| [getPreleveledStart()](#getPreleveledStart--) | Gets a value of PreleveledStart. |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Gets an object containing Primavera-specific properties for a task read from Primavera file. |
| [getPriority()](#getPriority--) | Gets a value of Priority. |
| [getRecurringInfo()](#getRecurringInfo--) | Gets the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null; |
| [getRegularWork()](#getRegularWork--) | Gets a value of RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Gets a value of RemainingCost. |
| [getRemainingDuration()](#getRemainingDuration--) | Gets a value of RemainingDuration. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Gets a value of RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Gets a value of RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Gets a value of RemainingWork. |
| [getResume()](#getResume--) | Gets a value of Resume. |
| [getSV()](#getSV--) | The earned value schedule variance, through the project status date. |
| [getSplitParts()](#getSplitParts--) | Gets a SplitPart collection that represents the portions of a task. |
| [getStart()](#getStart--) | Gets a value of Start. |
| [getStartSlack()](#getStartSlack--) | Gets a value of StartSlack. |
| [getStartText()](#getStartText--) | Gets a value of StartText. |
| [getStartVariance()](#getStartVariance--) | Gets a value of StartVariance. |
| [getStatus()](#getStatus--) | Gets task status. |
| [getStatusManager()](#getStatusManager--) | Gets a value of StatusManager. |
| [getStop()](#getStop--) | Gets a value of Stop. |
| [getSubprojectName()](#getSubprojectName--) | Gets a value of SubprojectName. |
| [getSuccessors()](#getSuccessors--) | Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all successors of this Task object. |
| [getTimephasedData()](#getTimephasedData--) | Gets a TimephasedDataCollection object of this task. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified time-phased data type. |
| [getTotalSlack()](#getTotalSlack--) | Gets a value of TotalSlack. |
| [getType()](#getType--) | Gets a value of Type. |
| [getUid()](#getUid--) | Gets a value of Uid. |
| [getWBS()](#getWBS--) | Gets a value of WBS. |
| [getWBSLevel()](#getWBSLevel--) | Gets a value of WBSLevel. |
| [getWarning()](#getWarning--) | Gets a value indicating whether Warning is set or not. |
| [getWork()](#getWork--) | Gets a value of Work. |
| [getWorkVariance()](#getWorkVariance--) | Gets a value of WorkVariance. |
| [hasChildren()](#hasChildren--) | Gets a value indicating that this task has children. |
| [hashCode()](#hashCode--) | Returns a hash code value for this Task. |
| [isActive()](#isActive--) | Gets a value indicating whether IsActive is set or not. |
| [isCritical()](#isCritical--) | Gets a value indicating whether IsCritical is set or not. |
| [isEffortDriven()](#isEffortDriven--) | Gets a value indicating whether IsEffortDriven is set or not. |
| [isEstimated()](#isEstimated--) | Gets a value indicating whether IsEstimated is set or not. |
| [isExpanded()](#isExpanded--) | Gets a value indicating whether IsExpanded is set or not. |
| [isExternalTask()](#isExternalTask--) | Gets a value indicating whether IsExternalTask is set or not. |
| [isManual()](#isManual--) | Gets a value indicating whether IsManual is set or not. |
| [isMarked()](#isMarked--) | Gets a value indicating whether IsMarked is set or not. |
| [isMilestone()](#isMilestone--) | Gets a value indicating whether IsMilestone is set or not. |
| [isNull()](#isNull--) | Gets a value indicating whether IsNull is set or not. |
| [isOverallocated()](#isOverallocated--) | Gets a value indicating whether IsOverallocated is set or not. |
| [isPublished()](#isPublished--) | Gets a value indicating whether IsPublished is set or not. |
| [isRecurring()](#isRecurring--) | Gets a value indicating whether IsRecurring is set or not. |
| [isResumeValid()](#isResumeValid--) | Gets a value indicating whether IsResumeValid is set or not. |
| [isRollup()](#isRollup--) | Gets a value indicating whether IsRollup is set or not. |
| [isSubproject()](#isSubproject--) | Gets a value indicating whether IsSubproject is set or not. |
| [isSubprojectReadOnly()](#isSubprojectReadOnly--) | Gets a value indicating whether IsSubprojectReadOnly is set or not. |
| [isSummary()](#isSummary--) | Gets a value indicating whether IsSummary is set or not. |
| [moveToSibling(Task beforeTask)](#moveToSibling-com.aspose.tasks.Task-) | Moves the current task at the same Outline Level before the specified task. |
| [moveToSibling(int beforeTaskId)](#moveToSibling-int-) | Moves the current task at the same Outline Level before a task with the specified Id. |
| [outlineIndent()](#outlineIndent--) | Indents a task in the outline. |
| [outlineOutdent()](#outlineOutdent--) | Promotes a task in the outline. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Recursively collects all child tasks of this task. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Maps the specified property to the specified value in this container. |
| [setACWP(double value)](#setACWP-double-) | Sets a value of ACWP. |
| [setActive(NullableBool value)](#setActive-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsActive is set or not. |
| [setActivityId(String value)](#setActivityId-java.lang.String-) | Represents activity id field - a task's unique identifier used by Primavera. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Sets a value of ActualCost. |
| [setActualDuration(Duration value)](#setActualDuration-com.aspose.tasks.Duration-) | Sets a value of ActualDuration. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Sets a value of ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Sets a value of ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Sets a value of ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Sets a value of ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Sets a value of ActualWorkProtected. |
| [setBCWP(double value)](#setBCWP-double-) | Sets a value of BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Sets a value of BCWS. |
| [setBaselines(TaskBaselineCollection value)](#setBaselines-com.aspose.tasks.TaskBaselineCollection-) | Sets the collection of baseline values of the task. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Sets a value of BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Sets a value of BudgetWork. |
| [setCV(double value)](#setCV-double-) | Sets a value of CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Sets a value of Calendar. |
| [setCommitmentFinish(Date value)](#setCommitmentFinish-java.util.Date-) | Sets a value of CommitmentFinish. |
| [setCommitmentStart(Date value)](#setCommitmentStart-java.util.Date-) | Sets a value of CommitmentStart. |
| [setCommitmentType(int value)](#setCommitmentType-int-) | Sets a value of CommitmentType. |
| [setConstraintDate(Date value)](#setConstraintDate-java.util.Date-) | Sets a value of ConstraintDate. |
| [setConstraintType(int value)](#setConstraintType-int-) | Sets a value of ConstraintType. |
| [setContact(String value)](#setContact-java.lang.String-) | Sets a value of Contact. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sets a value of Cost. |
| [setCostVariance(double value)](#setCostVariance-double-) | Sets a value of CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Sets a value of Created. |
| [setCritical(NullableBool value)](#setCritical-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsCritical is set or not. |
| [setDeadline(Date value)](#setDeadline-java.util.Date-) | Sets a value of Deadline. |
| [setDisplayAsSummary(NullableBool value)](#setDisplayAsSummary-com.aspose.tasks.NullableBool-) | Sets a value indicating whether DisplayAsSummary is set or not. |
| [setDisplayOnTimeline(boolean value)](#setDisplayOnTimeline-boolean-) | Sets a value indicating whether DisplayOnTimeline is set or not. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Sets a value of Duration. |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | Sets a value of DurationFormat. |
| [setDurationText(String value)](#setDurationText-java.lang.String-) | Sets a value of DurationText. |
| [setDurationVariance(Duration value)](#setDurationVariance-com.aspose.tasks.Duration-) | Sets a value of DurationVariance. |
| [setEarlyFinish(Date value)](#setEarlyFinish-java.util.Date-) | Sets a value of EarlyFinish. |
| [setEarlyStart(Date value)](#setEarlyStart-java.util.Date-) | Sets a value of EarlyStart. |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | Sets a value of EarnedValueMethod. |
| [setEffortDriven(NullableBool value)](#setEffortDriven-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsEffortDriven is set or not. |
| [setEstimated(NullableBool value)](#setEstimated-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsEstimated is set or not. |
| [setExpanded(NullableBool value)](#setExpanded-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsExpanded is set or not. |
| [setExternalId(int value)](#setExternalId-int-) | Sets a value of ExternalId. |
| [setExternalTask(boolean value)](#setExternalTask-boolean-) | Sets a value indicating whether IsExternalTask is set or not. |
| [setExternalTaskProject(String value)](#setExternalTaskProject-java.lang.String-) | Sets a value of ExternalTaskProject. |
| [setExternalUid(int value)](#setExternalUid-int-) | Set the external task's Unique identifier when the task is external. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sets a value of Finish. |
| [setFinishSlack(double value)](#setFinishSlack-double-) | Sets a value of FinishSlack. |
| [setFinishText(String value)](#setFinishText-java.lang.String-) | Sets a value of FinishText. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Sets a value of FinishVariance. |
| [setFixedCost(double value)](#setFixedCost-double-) | Sets a value of FixedCost. |
| [setFixedCostAccrual(int value)](#setFixedCostAccrual-int-) | Sets a value of FixedCostAccrual. |
| [setFreeSlack(double value)](#setFreeSlack-double-) | Sets a value of FreeSlack. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Sets a value of Guid. |
| [setHideBar(NullableBool value)](#setHideBar-com.aspose.tasks.NullableBool-) | Sets a value indicating whether HideBar is set or not. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Sets the title or explanatory text for a hyperlink associated with a task. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Sets the address for a hyperlink associated with a task. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Sets the specific location in a document in a hyperlink associated with a task. |
| [setId(int value)](#setId-int-) | Sets a value of Id. |
| [setIgnoreResourceCalendar(NullableBool value)](#setIgnoreResourceCalendar-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IgnoreResourceCalendar is set or not. |
| [setIgnoreWarnings(boolean value)](#setIgnoreWarnings-boolean-) | Sets a value indicating whether IgnoreWarnings is set or not. |
| [setLateFinish(Date value)](#setLateFinish-java.util.Date-) | Sets a value of LateFinish. |
| [setLateStart(Date value)](#setLateStart-java.util.Date-) | Sets a value of LateStart. |
| [setLevelAssignments(NullableBool value)](#setLevelAssignments-com.aspose.tasks.NullableBool-) | Sets a value indicating whether LevelAssignments is set or not. |
| [setLevelingCanSplit(NullableBool value)](#setLevelingCanSplit-com.aspose.tasks.NullableBool-) | Sets a value indicating whether LevelingCanSplit is set or not. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Sets a value of LevelingDelay. |
| [setManual(NullableBool value)](#setManual-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsManual is set or not. |
| [setManualDuration(Duration value)](#setManualDuration-com.aspose.tasks.Duration-) | Sets a value of ManualDuration. |
| [setManualFinish(Date value)](#setManualFinish-java.util.Date-) | Sets a value of ManualFinish. |
| [setManualStart(Date value)](#setManualStart-java.util.Date-) | Sets a value of ManualStart. |
| [setMarked(boolean value)](#setMarked-boolean-) | Sets a value indicating whether IsMarked is set or not. |
| [setMilestone(NullableBool value)](#setMilestone-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsMilestone is set or not. |
| [setName(String value)](#setName-java.lang.String-) | Sets a value of Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Sets a value of NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Sets a value of NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsNull is set or not. |
| [setOutlineCodes(OutlineCodeCollection value)](#setOutlineCodes-com.aspose.tasks.OutlineCodeCollection-) | Sets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |
| [setOutlineLevel(int value)](#setOutlineLevel-int-) | Sets a value of OutlineLevel. |
| [setOutlineNumber(String value)](#setOutlineNumber-java.lang.String-) | Sets a value of OutlineNumber. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsOverallocated is set or not. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Sets a value of OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of OvertimeWork. |
| [setPercentComplete(int value)](#setPercentComplete-int-) | Sets a value of PercentComplete. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Sets a value of PercentWorkComplete. |
| [setPhysicalPercentComplete(int value)](#setPhysicalPercentComplete-int-) | Sets a value of PhysicalPercentComplete. |
| [setPreleveledFinish(Date value)](#setPreleveledFinish-java.util.Date-) | Sets a value of PreleveledFinish. |
| [setPreleveledStart(Date value)](#setPreleveledStart-java.util.Date-) | Sets a value of PreleveledStart. |
| [setPriority(int value)](#setPriority-int-) | Sets a value of Priority. |
| [setPublished(NullableBool value)](#setPublished-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsPublished is set or not. |
| [setRecurring(NullableBool value)](#setRecurring-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsRecurring is set or not. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Sets a value of RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Sets a value of RemainingCost. |
| [setRemainingDuration(Duration value)](#setRemainingDuration-com.aspose.tasks.Duration-) | Sets a value of RemainingDuration. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Sets a value of RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Sets a value of RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Sets a value of RemainingWork. |
| [setResume(Date value)](#setResume-java.util.Date-) | Sets a value of Resume. |
| [setResumeValid(NullableBool value)](#setResumeValid-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsResumeValid is set or not. |
| [setRollup(NullableBool value)](#setRollup-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsRollup is set or not. |
| [setSV(double value)](#setSV-double-) | The earned value schedule variance, through the project status date. |
| [setStart(Date value)](#setStart-java.util.Date-) | Sets a value of Start. |
| [setStartSlack(double value)](#setStartSlack-double-) | Sets a value of StartSlack. |
| [setStartText(String value)](#setStartText-java.lang.String-) | Sets a value of StartText. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Sets a value of StartVariance. |
| [setStatusManager(String value)](#setStatusManager-java.lang.String-) | Sets a value of StatusManager. |
| [setStop(Date value)](#setStop-java.util.Date-) | Sets a value of Stop. |
| [setSubproject(boolean value)](#setSubproject-boolean-) | Sets a value indicating whether IsSubproject is set or not. |
| [setSubprojectName(String value)](#setSubprojectName-java.lang.String-) | Sets a value of SubprojectName. |
| [setSubprojectReadOnly(NullableBool value)](#setSubprojectReadOnly-com.aspose.tasks.NullableBool-) | Sets a value indicating whether IsSubprojectReadOnly is set or not. |
| [setSummary(boolean value)](#setSummary-boolean-) | Sets a value indicating whether IsSummary is set or not. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets a TimephasedDataCollection object of this task. |
| [setTotalSlack(double value)](#setTotalSlack-double-) | Sets a value of TotalSlack. |
| [setType(int value)](#setType-int-) | Sets a value of Type. |
| [setUid(int value)](#setUid-int-) | Sets a value of Uid. |
| [setWBS(String value)](#setWBS-java.lang.String-) | Sets a value of WBS. |
| [setWBSLevel(String value)](#setWBSLevel-java.lang.String-) | Sets a value of WBSLevel. |
| [setWarning(boolean value)](#setWarning-boolean-) | Sets a value indicating whether Warning is set or not. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Sets a value of Work. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Sets a value of WorkVariance. |
| [toString()](#toString--) | Returns short string representation of a task. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key. |

**Returns:**
T - the value to which the property is mapped in this container.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key. |
| val | T | the value. |

### deepClone() {#deepClone--}
```
public final Object deepClone()
```


Creates full copy of a task without subtasks.

**Returns:**
java.lang.Object - Created copy of a task.
### delete() {#delete--}
```
public final void delete()
```


Deletes a task from parent project tasks collection and all its assignments.

### equals(Task other) {#equals-com.aspose.tasks.Task-}
```
public final boolean equals(Task other)
```


Returns a value indicating whether this instance is equal to a specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Task](../../com.aspose.tasks/task) | The specified task to compare with this instance. |

**Returns:**
boolean - returns true if the specified task and this instance have equal unique ids.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The specified object to compare with this instance. |

**Returns:**
boolean - returns true if the specified task and this instance have equal unique ids.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Gets a value of ACWP.

**Returns:**
double - a value of ACWP.
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects).

**Returns:**
java.lang.String - a value of ActivityId.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Gets a value of ActualCost.

**Returns:**
java.math.BigDecimal - a value of ActualCost.
### getActualDuration() {#getActualDuration--}
```
public final Duration getActualDuration()
```


Gets a value of ActualDuration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualDuration.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Gets a value of ActualFinish.

**Returns:**
java.util.Date - a value of ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Gets a value of ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - a value of ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Gets a value of ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Gets a value of ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Gets a value of ActualStart.

**Returns:**
java.util.Date - a value of ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Gets a value of ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Gets a value of ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Gets a collection of resource assignments for this object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Gets a value of BCWP.

**Returns:**
double - a value of BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Gets a value of BCWS.

**Returns:**
double - a value of BCWS.
### getBaselines() {#getBaselines--}
```
public final TaskBaselineCollection getBaselines()
```


Gets the collection of baseline values of the task.

**Returns:**
[TaskBaselineCollection](../../com.aspose.tasks/taskbaselinecollection) - the collection of baseline values of the task.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Gets a value of BudgetCost.

**Returns:**
java.math.BigDecimal - a value of BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Gets a value of BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Gets a value of CV.

**Returns:**
double - a value of CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Gets a value of Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getChildren() {#getChildren--}
```
public final TaskCollection getChildren()
```


Gets a child task collection of this object. TaskCollection object which represents children tasks.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a child task collection of this object.
### getCommitmentFinish() {#getCommitmentFinish--}
```
public final Date getCommitmentFinish()
```


Gets a value of CommitmentFinish.

**Returns:**
java.util.Date - a value of CommitmentFinish.
### getCommitmentStart() {#getCommitmentStart--}
```
public final Date getCommitmentStart()
```


Gets a value of CommitmentStart.

**Returns:**
java.util.Date - a value of CommitmentStart.
### getCommitmentType() {#getCommitmentType--}
```
public final int getCommitmentType()
```


Gets a value of CommitmentType.

**Returns:**
int - a value of CommitmentType.
### getConstraintDate() {#getConstraintDate--}
```
public final Date getConstraintDate()
```


Gets a value of ConstraintDate.

**Returns:**
java.util.Date - a value of ConstraintDate.
### getConstraintType() {#getConstraintType--}
```
public final int getConstraintType()
```


Gets a value of ConstraintType.

**Returns:**
int - a value of ConstraintType.
### getContact() {#getContact--}
```
public final String getContact()
```


Gets a value of Contact.

**Returns:**
java.lang.String - a value of Contact.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Gets a value of Cost.

**Returns:**
java.math.BigDecimal - a value of Cost.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Gets a value of CostVariance.

**Returns:**
double - a value of CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Gets a value of Created.

**Returns:**
java.util.Date - a value of Created.
### getDeadline() {#getDeadline--}
```
public final Date getDeadline()
```


Gets a value of Deadline.

**Returns:**
java.util.Date - a value of Deadline.
### getDisplayAsSummary() {#getDisplayAsSummary--}
```
public final NullableBool getDisplayAsSummary()
```


Gets a value indicating whether DisplayAsSummary is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether DisplayAsSummary is set or not.
### getDisplayOnTimeline() {#getDisplayOnTimeline--}
```
public final boolean getDisplayOnTimeline()
```


Gets a value indicating whether DisplayOnTimeline is set or not.

**Returns:**
boolean - a value indicating whether DisplayOnTimeline is set or not.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Gets a value of Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Duration.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


Gets a value of DurationFormat.

**Returns:**
byte - a value of DurationFormat.
### getDurationText() {#getDurationText--}
```
public final String getDurationText()
```


Gets a value of DurationText.

**Returns:**
java.lang.String - a value of DurationText.
### getDurationVariance() {#getDurationVariance--}
```
public final Duration getDurationVariance()
```


Gets a value of DurationVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of DurationVariance.
### getEarlyFinish() {#getEarlyFinish--}
```
public final Date getEarlyFinish()
```


Gets a value of EarlyFinish.

**Returns:**
java.util.Date - a value of EarlyFinish.
### getEarlyStart() {#getEarlyStart--}
```
public final Date getEarlyStart()
```


Gets a value of EarlyStart.

**Returns:**
java.util.Date - a value of EarlyStart.
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


Gets a value of EarnedValueMethod.

**Returns:**
int - a value of EarnedValueMethod.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets ExtendedAttributeCollection object containing the values of an extended attribute.

--------------------

Two pieces of data are necessary - a pointer back to the extended attribute table which is specified either by the unique ID or the Field ID, and the value which is specified either with the value, or a pointer back to the value list.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - ExtendedAttributeCollection object containing the values of an extended attribute.
### getExternalId() {#getExternalId--}
```
public final int getExternalId()
```


Gets a value of ExternalId.

**Returns:**
int - a value of ExternalId.
### getExternalTaskProject() {#getExternalTaskProject--}
```
public final String getExternalTaskProject()
```


Gets a value of ExternalTaskProject.

**Returns:**
java.lang.String - a value of ExternalTaskProject.
### getExternalUid() {#getExternalUid--}
```
public final int getExternalUid()
```


Gets the external task's Unique identifier when the task is external.

**Returns:**
int - the external task's Unique identifier when the task is external.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Gets a value of Finish.

**Returns:**
java.util.Date - a value of Finish.
### getFinishSlack() {#getFinishSlack--}
```
public final double getFinishSlack()
```


Gets a value of FinishSlack.

**Returns:**
double - a value of FinishSlack.
### getFinishText() {#getFinishText--}
```
public final String getFinishText()
```


Gets a value of FinishText.

**Returns:**
java.lang.String - a value of FinishText.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Gets a value of FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Gets a value of FixedCost.

**Returns:**
double - a value of FixedCost.
### getFixedCostAccrual() {#getFixedCostAccrual--}
```
public final int getFixedCostAccrual()
```


Gets a value of FixedCostAccrual.

**Returns:**
int - a value of FixedCostAccrual.
### getFreeSlack() {#getFreeSlack--}
```
public final double getFreeSlack()
```


Gets a value of FreeSlack.

**Returns:**
double - a value of FreeSlack.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets a value of Guid.

**Returns:**
java.lang.String - a value of Guid.
### getHideBar() {#getHideBar--}
```
public final NullableBool getHideBar()
```


Gets a value indicating whether HideBar is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HideBar is set or not.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Gets the title or explanatory text for a hyperlink associated with a task.

**Returns:**
java.lang.String - the title or explanatory text for a hyperlink associated with a task.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Gets the address for a hyperlink associated with a task.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Returns:**
java.lang.String - the address for a hyperlink associated with a task.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Gets the specific location in a document in a hyperlink associated with a task.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Returns:**
java.lang.String - the specific location in a document in a hyperlink associated with a task.
### getId() {#getId--}
```
public final int getId()
```


Gets a value of Id.

**Returns:**
int - a value of Id.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final NullableBool getIgnoreResourceCalendar()
```


Gets a value indicating whether IgnoreResourceCalendar is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IgnoreResourceCalendar is set or not.
### getIgnoreWarnings() {#getIgnoreWarnings--}
```
public final boolean getIgnoreWarnings()
```


Gets a value indicating whether IgnoreWarnings is set or not.

**Returns:**
boolean - a value indicating whether IgnoreWarnings is set or not.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Reserved for internal usage.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLateFinish() {#getLateFinish--}
```
public final Date getLateFinish()
```


Gets a value of LateFinish.

**Returns:**
java.util.Date - a value of LateFinish.
### getLateStart() {#getLateStart--}
```
public final Date getLateStart()
```


Gets a value of LateStart.

**Returns:**
java.util.Date - a value of LateStart.
### getLevelAssignments() {#getLevelAssignments--}
```
public final NullableBool getLevelAssignments()
```


Gets a value indicating whether LevelAssignments is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether LevelAssignments is set or not.
### getLevelingCanSplit() {#getLevelingCanSplit--}
```
public final NullableBool getLevelingCanSplit()
```


Gets a value indicating whether LevelingCanSplit is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether LevelingCanSplit is set or not.
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Gets a value of LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getManualDuration() {#getManualDuration--}
```
public final Duration getManualDuration()
```


Gets a value of ManualDuration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ManualDuration.
### getManualFinish() {#getManualFinish--}
```
public final Date getManualFinish()
```


Gets a value of ManualFinish.

**Returns:**
java.util.Date - a value of ManualFinish.
### getManualStart() {#getManualStart--}
```
public final Date getManualStart()
```


Gets a value of ManualStart.

**Returns:**
java.util.Date - a value of ManualStart.
### getName() {#getName--}
```
public final String getName()
```


Gets a value of Name.

**Returns:**
java.lang.String - a value of Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Gets a value of NotesRTF.

**Returns:**
java.lang.String - a value of NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Gets a value of NotesText.

**Returns:**
java.lang.String - a value of NotesText.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeCollection getOutlineCodes()
```


Gets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.
### getOutlineLevel() {#getOutlineLevel--}
```
public final int getOutlineLevel()
```


Gets a value of OutlineLevel.

**Returns:**
int - a value of OutlineLevel.
### getOutlineNumber() {#getOutlineNumber--}
```
public final String getOutlineNumber()
```


Gets a value of OutlineNumber.

**Returns:**
java.lang.String - a value of OutlineNumber.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Gets a value of OvertimeCost.

**Returns:**
java.math.BigDecimal - a value of OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Gets a value of OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of a task.

--------------------

Call Project.UpdateReferences to update these properties.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of a task.
### getParentTask() {#getParentTask--}
```
public final Task getParentTask()
```


Gets the parent task of a task.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of a task.
### getPercentComplete() {#getPercentComplete--}
```
public final int getPercentComplete()
```


Gets a value of PercentComplete.

**Returns:**
int - a value of PercentComplete.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Gets a value of PercentWorkComplete.

**Returns:**
int - a value of PercentWorkComplete.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final int getPhysicalPercentComplete()
```


Gets a value of PhysicalPercentComplete.

**Returns:**
int - a value of PhysicalPercentComplete.
### getPredecessors() {#getPredecessors--}
```
public final TaskCollection getPredecessors()
```


Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all predecessors of this Task object.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - Read-only instance of [TaskCollection](../../com.aspose.tasks/taskcollection) class.
### getPreleveledFinish() {#getPreleveledFinish--}
```
public final Date getPreleveledFinish()
```


Gets a value of PreleveledFinish.

**Returns:**
java.util.Date - a value of PreleveledFinish.
### getPreleveledStart() {#getPreleveledStart--}
```
public final Date getPreleveledStart()
```


Gets a value of PreleveledStart.

**Returns:**
java.util.Date - a value of PreleveledStart.
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraTaskProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a task read from Primavera file.

**Returns:**
[PrimaveraTaskProperties](../../com.aspose.tasks/primaverataskproperties) - an object containing Primavera-specific properties for a task read from Primavera file.
### getPriority() {#getPriority--}
```
public final int getPriority()
```


Gets a value of Priority.

**Returns:**
int - a value of Priority.
### getRecurringInfo() {#getRecurringInfo--}
```
public final RecurringTaskInfo getRecurringInfo()
```


Gets the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null;

--------------------

The info for the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) is present in mpp file format only.

**Returns:**
[RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) - the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null;
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Gets a value of RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Gets a value of RemainingCost.

**Returns:**
java.math.BigDecimal - a value of RemainingCost.
### getRemainingDuration() {#getRemainingDuration--}
```
public final Duration getRemainingDuration()
```


Gets a value of RemainingDuration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingDuration.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Gets a value of RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - a value of RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Gets a value of RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Gets a value of RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResume() {#getResume--}
```
public final Date getResume()
```


Gets a value of Resume.

**Returns:**
java.util.Date - a value of Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS.

**Returns:**
double - a value of SV.
### getSplitParts() {#getSplitParts--}
```
public final SplitPartCollection getSplitParts()
```


Gets a SplitPart collection that represents the portions of a task.

**Returns:**
[SplitPartCollection](../../com.aspose.tasks/splitpartcollection) - a SplitPart collection that represents the portions of a task.
### getStart() {#getStart--}
```
public final Date getStart()
```


Gets a value of Start.

**Returns:**
java.util.Date - a value of Start.
### getStartSlack() {#getStartSlack--}
```
public final double getStartSlack()
```


Gets a value of StartSlack.

**Returns:**
double - a value of StartSlack.
### getStartText() {#getStartText--}
```
public final String getStartText()
```


Gets a value of StartText.

**Returns:**
java.lang.String - a value of StartText.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Gets a value of StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Gets task status.

**Returns:**
int - task status.
### getStatusManager() {#getStatusManager--}
```
public final String getStatusManager()
```


Gets a value of StatusManager.

**Returns:**
java.lang.String - a value of StatusManager.
### getStop() {#getStop--}
```
public final Date getStop()
```


Gets a value of Stop.

**Returns:**
java.util.Date - a value of Stop.
### getSubprojectName() {#getSubprojectName--}
```
public final String getSubprojectName()
```


Gets a value of SubprojectName.

**Returns:**
java.lang.String - a value of SubprojectName.
### getSuccessors() {#getSuccessors--}
```
public final TaskCollection getSuccessors()
```


Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all successors of this Task object.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - Read-only instance of [TaskCollection](../../com.aspose.tasks/taskcollection) class.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets a TimephasedDataCollection object of this task. The time phased data block associated with a task.

--------------------

Reading supported for XML format only.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection object of this task.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata) to be filled in.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified time-phased data type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | byte | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - A [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified timephased data type.
### getTotalSlack() {#getTotalSlack--}
```
public final double getTotalSlack()
```


Gets a value of TotalSlack.

**Returns:**
double - a value of TotalSlack.
### getType() {#getType--}
```
public final int getType()
```


Gets a value of Type.

**Returns:**
int - a value of Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets a value of Uid.

**Returns:**
int - a value of Uid.
### getWBS() {#getWBS--}
```
public final String getWBS()
```


Gets a value of WBS.

**Returns:**
java.lang.String - a value of WBS.
### getWBSLevel() {#getWBSLevel--}
```
public final String getWBSLevel()
```


Gets a value of WBSLevel.

**Returns:**
java.lang.String - a value of WBSLevel.
### getWarning() {#getWarning--}
```
public final boolean getWarning()
```


Gets a value indicating whether Warning is set or not.

**Returns:**
boolean - a value indicating whether Warning is set or not.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Gets a value of Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Gets a value of WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Gets a value indicating that this task has children.

**Returns:**
boolean - a value indicating that this task has children.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for this Task.

**Returns:**
int - returns a hash code value for this object.
### isActive() {#isActive--}
```
public final NullableBool isActive()
```


Gets a value indicating whether IsActive is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsActive is set or not.
### isCritical() {#isCritical--}
```
public final NullableBool isCritical()
```


Gets a value indicating whether IsCritical is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCritical is set or not.
### isEffortDriven() {#isEffortDriven--}
```
public final NullableBool isEffortDriven()
```


Gets a value indicating whether IsEffortDriven is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEffortDriven is set or not.
### isEstimated() {#isEstimated--}
```
public final NullableBool isEstimated()
```


Gets a value indicating whether IsEstimated is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEstimated is set or not.
### isExpanded() {#isExpanded--}
```
public final NullableBool isExpanded()
```


Gets a value indicating whether IsExpanded is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsExpanded is set or not.
### isExternalTask() {#isExternalTask--}
```
public final boolean isExternalTask()
```


Gets a value indicating whether IsExternalTask is set or not.

**Returns:**
boolean - a value indicating whether IsExternalTask is set or not.
### isManual() {#isManual--}
```
public final NullableBool isManual()
```


Gets a value indicating whether IsManual is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsManual is set or not.
### isMarked() {#isMarked--}
```
public final boolean isMarked()
```


Gets a value indicating whether IsMarked is set or not.

**Returns:**
boolean - a value indicating whether IsMarked is set or not.
### isMilestone() {#isMilestone--}
```
public final NullableBool isMilestone()
```


Gets a value indicating whether IsMilestone is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsMilestone is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Gets a value indicating whether IsNull is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isOverallocated() {#isOverallocated--}
```
public final NullableBool isOverallocated()
```


Gets a value indicating whether IsOverallocated is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsOverallocated is set or not.
### isPublished() {#isPublished--}
```
public final NullableBool isPublished()
```


Gets a value indicating whether IsPublished is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsPublished is set or not.
### isRecurring() {#isRecurring--}
```
public final NullableBool isRecurring()
```


Gets a value indicating whether IsRecurring is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsRecurring is set or not.
### isResumeValid() {#isResumeValid--}
```
public final NullableBool isResumeValid()
```


Gets a value indicating whether IsResumeValid is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsResumeValid is set or not.
### isRollup() {#isRollup--}
```
public final NullableBool isRollup()
```


Gets a value indicating whether IsRollup is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsRollup is set or not.
### isSubproject() {#isSubproject--}
```
public final boolean isSubproject()
```


Gets a value indicating whether IsSubproject is set or not.

**Returns:**
boolean - a value indicating whether IsSubproject is set or not.
### isSubprojectReadOnly() {#isSubprojectReadOnly--}
```
public final NullableBool isSubprojectReadOnly()
```


Gets a value indicating whether IsSubprojectReadOnly is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsSubprojectReadOnly is set or not.
### isSummary() {#isSummary--}
```
public final boolean isSummary()
```


Gets a value indicating whether IsSummary is set or not.

**Returns:**
boolean - a value indicating whether IsSummary is set or not.
### moveToSibling(Task beforeTask) {#moveToSibling-com.aspose.tasks.Task-}
```
public final void moveToSibling(Task beforeTask)
```


Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beforeTask | [Task](../../com.aspose.tasks/task) | Task before which the current task will be inserted. |

### moveToSibling(int beforeTaskId) {#moveToSibling-int-}
```
public final void moveToSibling(int beforeTaskId)
```


Moves the current task at the same Outline Level before a task with the specified Id. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beforeTaskId | int | Id ([Tsk.ID](../../com.aspose.tasks/tsk\#ID)) of a task before which the current task will be inserted. |

### outlineIndent() {#outlineIndent--}
```
public final void outlineIndent()
```


Indents a task in the outline.

### outlineOutdent() {#outlineOutdent--}
```
public final void outlineOutdent()
```


Promotes a task in the outline.

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final Iterable<Task> selectAllChildTasks()
```


Recursively collects all child tasks of this task.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - A list of child tasks of this task.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key. |
| val | java.util.Date | the value. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Sets a value of ACWP.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of ACWP. |

### setActive(NullableBool value) {#setActive-com.aspose.tasks.NullableBool-}
```
public final void setActive(NullableBool value)
```


Sets a value indicating whether IsActive is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsActive is set or not. |

### setActivityId(String value) {#setActivityId-java.lang.String-}
```
public final void setActivityId(String value)
```


Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of ActivityId. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Sets a value of ActualCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of ActualCost. |

### setActualDuration(Duration value) {#setActualDuration-com.aspose.tasks.Duration-}
```
public final void setActualDuration(Duration value)
```


Sets a value of ActualDuration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualDuration. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Sets a value of ActualFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Sets a value of ActualOvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Sets a value of ActualOvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Sets a value of ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Sets a value of ActualStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Sets a value of ActualWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Sets a value of ActualWorkProtected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ActualWorkProtected. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Sets a value of BCWP.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Sets a value of BCWS.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of BCWS. |

### setBaselines(TaskBaselineCollection value) {#setBaselines-com.aspose.tasks.TaskBaselineCollection-}
```
public final void setBaselines(TaskBaselineCollection value)
```


Sets the collection of baseline values of the task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBaselineCollection](../../com.aspose.tasks/taskbaselinecollection) | the collection of baseline values of the task. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Sets a value of BudgetCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Sets a value of BudgetWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Sets a value of CV.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCommitmentFinish(Date value) {#setCommitmentFinish-java.util.Date-}
```
public final void setCommitmentFinish(Date value)
```


Sets a value of CommitmentFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CommitmentFinish. |

### setCommitmentStart(Date value) {#setCommitmentStart-java.util.Date-}
```
public final void setCommitmentStart(Date value)
```


Sets a value of CommitmentStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CommitmentStart. |

### setCommitmentType(int value) {#setCommitmentType-int-}
```
public final void setCommitmentType(int value)
```


Sets a value of CommitmentType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CommitmentType. |

### setConstraintDate(Date value) {#setConstraintDate-java.util.Date-}
```
public final void setConstraintDate(Date value)
```


Sets a value of ConstraintDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ConstraintDate. |

### setConstraintType(int value) {#setConstraintType-int-}
```
public final void setConstraintType(int value)
```


Sets a value of ConstraintType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of ConstraintType. |

### setContact(String value) {#setContact-java.lang.String-}
```
public final void setContact(String value)
```


Sets a value of Contact.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Contact. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sets a value of Cost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of Cost. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Sets a value of CostVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Sets a value of Created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Created. |

### setCritical(NullableBool value) {#setCritical-com.aspose.tasks.NullableBool-}
```
public final void setCritical(NullableBool value)
```


Sets a value indicating whether IsCritical is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsCritical is set or not. |

### setDeadline(Date value) {#setDeadline-java.util.Date-}
```
public final void setDeadline(Date value)
```


Sets a value of Deadline.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Deadline. |

### setDisplayAsSummary(NullableBool value) {#setDisplayAsSummary-com.aspose.tasks.NullableBool-}
```
public final void setDisplayAsSummary(NullableBool value)
```


Sets a value indicating whether DisplayAsSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether DisplayAsSummary is set or not. |

### setDisplayOnTimeline(boolean value) {#setDisplayOnTimeline-boolean-}
```
public final void setDisplayOnTimeline(boolean value)
```


Sets a value indicating whether DisplayOnTimeline is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether DisplayOnTimeline is set or not. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Sets a value of Duration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of Duration. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setDurationText(String value) {#setDurationText-java.lang.String-}
```
public final void setDurationText(String value)
```


Sets a value of DurationText.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of DurationText. |

### setDurationVariance(Duration value) {#setDurationVariance-com.aspose.tasks.Duration-}
```
public final void setDurationVariance(Duration value)
```


Sets a value of DurationVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of DurationVariance. |

### setEarlyFinish(Date value) {#setEarlyFinish-java.util.Date-}
```
public final void setEarlyFinish(Date value)
```


Sets a value of EarlyFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of EarlyFinish. |

### setEarlyStart(Date value) {#setEarlyStart-java.util.Date-}
```
public final void setEarlyStart(Date value)
```


Sets a value of EarlyStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of EarlyStart. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setEffortDriven(NullableBool value) {#setEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setEffortDriven(NullableBool value)
```


Sets a value indicating whether IsEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsEffortDriven is set or not. |

### setEstimated(NullableBool value) {#setEstimated-com.aspose.tasks.NullableBool-}
```
public final void setEstimated(NullableBool value)
```


Sets a value indicating whether IsEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsEstimated is set or not. |

### setExpanded(NullableBool value) {#setExpanded-com.aspose.tasks.NullableBool-}
```
public final void setExpanded(NullableBool value)
```


Sets a value indicating whether IsExpanded is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsExpanded is set or not. |

### setExternalId(int value) {#setExternalId-int-}
```
public final void setExternalId(int value)
```


Sets a value of ExternalId.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of ExternalId. |

### setExternalTask(boolean value) {#setExternalTask-boolean-}
```
public final void setExternalTask(boolean value)
```


Sets a value indicating whether IsExternalTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IsExternalTask is set or not. |

### setExternalTaskProject(String value) {#setExternalTaskProject-java.lang.String-}
```
public final void setExternalTaskProject(String value)
```


Sets a value of ExternalTaskProject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of ExternalTaskProject. |

### setExternalUid(int value) {#setExternalUid-int-}
```
public final void setExternalUid(int value)
```


Set the external task's Unique identifier when the task is external.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the external task's Unique identifier when the task is external. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sets a value of Finish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Finish. |

### setFinishSlack(double value) {#setFinishSlack-double-}
```
public final void setFinishSlack(double value)
```


Sets a value of FinishSlack.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of FinishSlack. |

### setFinishText(String value) {#setFinishText-java.lang.String-}
```
public final void setFinishText(String value)
```


Sets a value of FinishText.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of FinishText. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Sets a value of FinishVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of FinishVariance. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Sets a value of FixedCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of FixedCost. |

### setFixedCostAccrual(int value) {#setFixedCostAccrual-int-}
```
public final void setFixedCostAccrual(int value)
```


Sets a value of FixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FixedCostAccrual. |

### setFreeSlack(double value) {#setFreeSlack-double-}
```
public final void setFreeSlack(double value)
```


Sets a value of FreeSlack.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of FreeSlack. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Guid. |

### setHideBar(NullableBool value) {#setHideBar-com.aspose.tasks.NullableBool-}
```
public final void setHideBar(NullableBool value)
```


Sets a value indicating whether HideBar is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HideBar is set or not. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Sets the title or explanatory text for a hyperlink associated with a task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the title or explanatory text for a hyperlink associated with a task. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Sets the address for a hyperlink associated with a task.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the address for a hyperlink associated with a task. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Sets the specific location in a document in a hyperlink associated with a task.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the specific location in a document in a hyperlink associated with a task. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Sets a value of Id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Id. |

### setIgnoreResourceCalendar(NullableBool value) {#setIgnoreResourceCalendar-com.aspose.tasks.NullableBool-}
```
public final void setIgnoreResourceCalendar(NullableBool value)
```


Sets a value indicating whether IgnoreResourceCalendar is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IgnoreResourceCalendar is set or not. |

### setIgnoreWarnings(boolean value) {#setIgnoreWarnings-boolean-}
```
public final void setIgnoreWarnings(boolean value)
```


Sets a value indicating whether IgnoreWarnings is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IgnoreWarnings is set or not. |

### setLateFinish(Date value) {#setLateFinish-java.util.Date-}
```
public final void setLateFinish(Date value)
```


Sets a value of LateFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LateFinish. |

### setLateStart(Date value) {#setLateStart-java.util.Date-}
```
public final void setLateStart(Date value)
```


Sets a value of LateStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LateStart. |

### setLevelAssignments(NullableBool value) {#setLevelAssignments-com.aspose.tasks.NullableBool-}
```
public final void setLevelAssignments(NullableBool value)
```


Sets a value indicating whether LevelAssignments is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether LevelAssignments is set or not. |

### setLevelingCanSplit(NullableBool value) {#setLevelingCanSplit-com.aspose.tasks.NullableBool-}
```
public final void setLevelingCanSplit(NullableBool value)
```


Sets a value indicating whether LevelingCanSplit is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether LevelingCanSplit is set or not. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Sets a value of LevelingDelay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of LevelingDelay. |

### setManual(NullableBool value) {#setManual-com.aspose.tasks.NullableBool-}
```
public final void setManual(NullableBool value)
```


Sets a value indicating whether IsManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsManual is set or not. |

### setManualDuration(Duration value) {#setManualDuration-com.aspose.tasks.Duration-}
```
public final void setManualDuration(Duration value)
```


Sets a value of ManualDuration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of ManualDuration. |

### setManualFinish(Date value) {#setManualFinish-java.util.Date-}
```
public final void setManualFinish(Date value)
```


Sets a value of ManualFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ManualFinish. |

### setManualStart(Date value) {#setManualStart-java.util.Date-}
```
public final void setManualStart(Date value)
```


Sets a value of ManualStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ManualStart. |

### setMarked(boolean value) {#setMarked-boolean-}
```
public final void setMarked(boolean value)
```


Sets a value indicating whether IsMarked is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IsMarked is set or not. |

### setMilestone(NullableBool value) {#setMilestone-com.aspose.tasks.NullableBool-}
```
public final void setMilestone(NullableBool value)
```


Sets a value indicating whether IsMilestone is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsMilestone is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Sets a value of NotesRTF.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Sets a value of NotesText.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Sets a value indicating whether IsNull is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsNull is set or not. |

### setOutlineCodes(OutlineCodeCollection value) {#setOutlineCodes-com.aspose.tasks.OutlineCodeCollection-}
```
public final void setOutlineCodes(OutlineCodeCollection value)
```


Sets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) | [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |

### setOutlineLevel(int value) {#setOutlineLevel-int-}
```
public final void setOutlineLevel(int value)
```


Sets a value of OutlineLevel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of OutlineLevel. |

### setOutlineNumber(String value) {#setOutlineNumber-java.lang.String-}
```
public final void setOutlineNumber(String value)
```


Sets a value of OutlineNumber.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of OutlineNumber. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Sets a value indicating whether IsOverallocated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsOverallocated is set or not. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Sets a value of OvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Sets a value of OvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of OvertimeWork. |

### setPercentComplete(int value) {#setPercentComplete-int-}
```
public final void setPercentComplete(int value)
```


Sets a value of PercentComplete.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of PercentComplete. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Sets a value of PercentWorkComplete.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of PercentWorkComplete. |

### setPhysicalPercentComplete(int value) {#setPhysicalPercentComplete-int-}
```
public final void setPhysicalPercentComplete(int value)
```


Sets a value of PhysicalPercentComplete.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of PhysicalPercentComplete. |

### setPreleveledFinish(Date value) {#setPreleveledFinish-java.util.Date-}
```
public final void setPreleveledFinish(Date value)
```


Sets a value of PreleveledFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of PreleveledFinish. |

### setPreleveledStart(Date value) {#setPreleveledStart-java.util.Date-}
```
public final void setPreleveledStart(Date value)
```


Sets a value of PreleveledStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of PreleveledStart. |

### setPriority(int value) {#setPriority-int-}
```
public final void setPriority(int value)
```


Sets a value of Priority.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Priority. |

### setPublished(NullableBool value) {#setPublished-com.aspose.tasks.NullableBool-}
```
public final void setPublished(NullableBool value)
```


Sets a value indicating whether IsPublished is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsPublished is set or not. |

### setRecurring(NullableBool value) {#setRecurring-com.aspose.tasks.NullableBool-}
```
public final void setRecurring(NullableBool value)
```


Sets a value indicating whether IsRecurring is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsRecurring is set or not. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Sets a value of RegularWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Sets a value of RemainingCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of RemainingCost. |

### setRemainingDuration(Duration value) {#setRemainingDuration-com.aspose.tasks.Duration-}
```
public final void setRemainingDuration(Duration value)
```


Sets a value of RemainingDuration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RemainingDuration. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Sets a value of RemainingOvertimeCost.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | a value of RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Sets a value of RemainingOvertimeWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Sets a value of RemainingWork.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of RemainingWork. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Sets a value of Resume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Resume. |

### setResumeValid(NullableBool value) {#setResumeValid-com.aspose.tasks.NullableBool-}
```
public final void setResumeValid(NullableBool value)
```


Sets a value indicating whether IsResumeValid is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsResumeValid is set or not. |

### setRollup(NullableBool value) {#setRollup-com.aspose.tasks.NullableBool-}
```
public final void setRollup(NullableBool value)
```


Sets a value indicating whether IsRollup is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsRollup is set or not. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Sets a value of Start.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Start. |

### setStartSlack(double value) {#setStartSlack-double-}
```
public final void setStartSlack(double value)
```


Sets a value of StartSlack.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of StartSlack. |

### setStartText(String value) {#setStartText-java.lang.String-}
```
public final void setStartText(String value)
```


Sets a value of StartText.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of StartText. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Sets a value of StartVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of StartVariance. |

### setStatusManager(String value) {#setStatusManager-java.lang.String-}
```
public final void setStatusManager(String value)
```


Sets a value of StatusManager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of StatusManager. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Sets a value of Stop.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of Stop. |

### setSubproject(boolean value) {#setSubproject-boolean-}
```
public final void setSubproject(boolean value)
```


Sets a value indicating whether IsSubproject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IsSubproject is set or not. |

### setSubprojectName(String value) {#setSubprojectName-java.lang.String-}
```
public final void setSubprojectName(String value)
```


Sets a value of SubprojectName.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of SubprojectName. |

### setSubprojectReadOnly(NullableBool value) {#setSubprojectReadOnly-com.aspose.tasks.NullableBool-}
```
public final void setSubprojectReadOnly(NullableBool value)
```


Sets a value indicating whether IsSubprojectReadOnly is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether IsSubprojectReadOnly is set or not. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Sets a value indicating whether IsSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether IsSummary is set or not. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets a TimephasedDataCollection object of this task. The time phased data block associated with a task.

--------------------

Reading supported for XML format only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | a TimephasedDataCollection object of this task. |

### setTotalSlack(double value) {#setTotalSlack-double-}
```
public final void setTotalSlack(double value)
```


Sets a value of TotalSlack.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of TotalSlack. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Sets a value of Type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Uid. |

### setWBS(String value) {#setWBS-java.lang.String-}
```
public final void setWBS(String value)
```


Sets a value of WBS.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of WBS. |

### setWBSLevel(String value) {#setWBSLevel-java.lang.String-}
```
public final void setWBSLevel(String value)
```


Sets a value of WBSLevel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of WBSLevel. |

### setWarning(boolean value) {#setWarning-boolean-}
```
public final void setWarning(boolean value)
```


Sets a value indicating whether Warning is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Warning is set or not. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Sets a value of Work.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of Work. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Sets a value of WorkVariance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | a value of WorkVariance. |

### toString() {#toString--}
```
public String toString()
```


Returns short string representation of a task. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents task object.
