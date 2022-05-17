---
title: Project
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.tasks/project/project/
---
## Project constructor (1 of 13)

Initializes a new instance of the [`Project`](../../project) class.

```csharp
public Project()
```

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (2 of 13)

Initializes a new instance of the [`Project`](../../project) class from a password protected template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |
| protectionPassword | String | Protection password. |

### Remarks

Reading password protected files currently supported for MSP 2003 file format only.

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (3 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (4 of 13)

Initializes a new instance of the [`Project`](../../project) class from the Stream with the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions) class.

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream of the Project Streamclass |
| options | PrimaveraReadOptions | the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions)class which allows to customize reading of Primavera formats (XER or XML). |

### See Also

* class [PrimaveraReadOptions](../../primaverareadoptions)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (5 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template (existent mpp or mpt file).

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from. |
| parseErrorHandler | ParseErrorCallback | the specified callback method to handle xml parse errors. |

### See Also

* delegate [ParseErrorCallback](../../parseerrorcallback)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (6 of 13)

Initializes a new instance of the [`Project`](../../project) class from a stream.

```csharp
public Project(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (7 of 13)

Initializes a new instance of the [`Project`](../../project) class from a StreamReader instance.

```csharp
public Project(StreamReader reader)
```

| Parameter | Type | Description |
| --- | --- | --- |
| reader | StreamReader | The stream reader where to load a template from. |

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (8 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template (existent MPP or MPT file) with the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions) class.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from |
| options | PrimaveraReadOptions | the specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions) class. |

### See Also

* class [PrimaveraReadOptions](../../primaverareadoptions)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (9 of 13)

Initializes a new instance of the [`Project`](../../project) class to read data from a database which is specified by the instance of the [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings) class.

```csharp
public Project(DbSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | DbSettings | the specified instance of the [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings) class. |

### See Also

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (10 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template(existent mpp or mpt file).

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |
| parseErrorHandler | ParseErrorCallback | the specified callback method to handle xml parse errors. |

### See Also

* delegate [ParseErrorCallback](../../parseerrorcallback)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (11 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template(existent mpp or mpt file).

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream to load a template from. |
| protectionPassword | String | Protection password. |

### Remarks

Reading password protected files currently supported for MSP 2003 file format only.

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (12 of 13)

Initializes a new instance of the [`Project`](../../project) class from a template (existent mpp or mpt file) with the specified instance of the [`LoadOptions`](../../loadoptions) class.

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | String | Path to template to create project from |
| options | LoadOptions | the specified instance of the [`LoadOptions`](../../loadoptions) class. |

### See Also

* class [LoadOptions](../../loadoptions)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project constructor (13 of 13)

Initializes a new instance of the [`Project`](../../project) class from the Stream with the specified instance of the [`LoadOptions`](../../loadoptions) class.

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream of the Project Streamclass |
| options | LoadOptions | the specified instance of the [`LoadOptions`](../../loadoptions)class |

### See Also

* class [LoadOptions](../../loadoptions)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
