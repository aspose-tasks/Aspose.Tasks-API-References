---
title: ProjectServerSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when project is saved to Project Server or Project Online.
type: docs
weight: 226
url: /java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Allows to specify additional options when project is saved to Project Server or Project Online.
## Constructors

| Constructor | Description |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Initializes a new instance of the [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Gets interval between queue job status requests. |
| [getProjectGuid()](#getProjectGuid--) | Gets unique identifier of a project. |
| [getProjectName()](#getProjectName--) | Gets name of a project which is displayed in Project Server \\ Project Online projects list. |
| [getTimeout()](#getTimeout--) | Gets timeout used when waiting for processing of save project request by a Project Server's queue processing service. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Sets interval between queue job status requests. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Sets unique identifier of a project. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Sets name of a project which is displayed in Project Server \\ Project Online projects list. |
| [setTimeout(double value)](#setTimeout-double-) | Sets timeout used when waiting for processing of save project request by a Project Server's queue processing service. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Initializes a new instance of the [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) class.

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Gets interval between queue job status requests. The default value is 2 seconds.

**Returns:**
double - interval between queue job status requests.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Gets unique identifier of a project. Should be unique within Project Server \\ Project Online instance.

**Returns:**
java.util.UUID - unique identifier of a project.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Gets name of a project which is displayed in Project Server \\ Project Online projects list. Should be unique within Project Server \\ Project Online instance. Is the value is omitted, the value of Prj.Name property will be used instead.

**Returns:**
java.lang.String - name of a project which is displayed in Project Server \\ Project Online projects list.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Gets timeout used when waiting for processing of save project request by a Project Server's queue processing service. The default value for this property is 1 minute.

--------------------

The processing time may be longer for large projects or in case when Project Server instance is too busy responding to other requests.

**Returns:**
double - timeout used when waiting for processing of save project request by a Project Server's queue processing service.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Sets interval between queue job status requests. The default value is 2 seconds.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | interval between queue job status requests. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Sets unique identifier of a project. Should be unique within Project Server \\ Project Online instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | unique identifier of a project. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Sets name of a project which is displayed in Project Server \\ Project Online projects list. Should be unique within Project Server \\ Project Online instance. Is the value is omitted, the value of Prj.Name property will be used instead.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | name of a project which is displayed in Project Server \\ Project Online projects list. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Sets timeout used when waiting for processing of save project request by a Project Server's queue processing service. The default value for this property is 1 minute.

--------------------

The processing time may be longer for large projects or in case when Project Server instance is too busy responding to other requests.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | timeout used when waiting for processing of save project request by a Project Server's queue processing service. |

