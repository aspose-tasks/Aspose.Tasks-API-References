---
title: PrimaveraProjectProperties
second_title: Aspose.Tasks for Java API Reference
description: Represents Primavera-specific properties for a project read from Primavera files XER of P6XML.
type: docs
weight: 201
url: /java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Represents Primavera-specific properties for a project read from Primavera files (XER of P6XML).
## Methods

| Method | Description |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Gets array of baseline projects of current project. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Gets Id of the current baseline project. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Gets a flag which defines whether to ignore activity relationships between projects. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Gets a flag which defines whether activities should me marked as critical when scheduling the project. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Gets an options which defines which calendar to use for scheduling Relationship Lag in Primavera projects |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Gets a flag which defines whether activity finish dates should be scheduled as the expected finish dates. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Gets array of baseline projects of current project. Is applicable to projects read from Primavera XML files containing exported baselines.

**Returns:**
com.aspose.tasks.Project[] - array of baseline projects of current project.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Gets Id of the current baseline project. Is applicable to projects read from Primavera XML files containing exported baselines.

**Returns:**
int - Id of the current baseline project.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Gets a flag which defines whether to ignore activity relationships between projects.

**Returns:**
boolean - a flag which defines whether to ignore activity relationships between projects.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Gets a flag which defines whether activities should me marked as critical when scheduling the project.

**Returns:**
boolean - a flag which defines whether activities should me marked as critical when scheduling the project.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Gets an options which defines which calendar to use for scheduling Relationship Lag in Primavera projects

**Returns:**
int - an options which defines which calendar to use for scheduling Relationship Lag in Primavera projects
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Gets a flag which defines whether activity finish dates should be scheduled as the expected finish dates.

**Returns:**
boolean - a flag which defines whether activity finish dates should be scheduled as the expected finish dates.
