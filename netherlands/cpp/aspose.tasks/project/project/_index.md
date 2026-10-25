---
title: "Aspose::Tasks::Project::Project constructor"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks voor C++"
description: "Initialiseert een nieuwe instantie van de Project‑klasse."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Initialiseert een nieuwe instantie van de Project‑klasse.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een met wachtwoord beveiligde sjabloon (bestaand mpp- of mpt-bestand).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parameter | Beschrijving |
| --- | --- |
| projectTemplate | Pad naar sjabloon om project van te maken. |
| protectionPassword | Beschermingswachtwoord. |

---

## Project (3 of 13) {#project_3}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parameter | Beschrijving |
| --- | --- |
| projectTemplate | Pad naar sjabloon om project van te maken. |

---

## Project (4 of 13) {#project_4}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit de Stream met de opgegeven instantie van de PrimaveraReadOptions-klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Beschrijving |
| --- | --- |
| stream | Stream van de Project System::IO::Stream-klasse |
| options | de opgegeven instantie van de PrimaveraReadOptions-klasse die het mogelijk maakt om het lezen van Primavera-formaten (XER of XML) aan te passen. |

---

## Project (5 of 13) {#project_5}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Beschrijving |
| --- | --- |
| projectTemplate | Pad naar sjabloon om project van te maken. |
| parseErrorHandler | de opgegeven callback-methode om xml-parsefouten af te handelen. |

---

## Project (6 of 13) {#project_6}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parameter | Beschrijving |
| --- | --- |
| stream | Stream om een sjabloon van te laden. |

---

## Project (7 of 13) {#project_7}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een StreamReader-instantie.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parameter | Beschrijving |
| --- | --- |
| reader | De streamlezer waar een sjabloon van geladen moet worden. |

---

## Project (8 of 13) {#project_8}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand MPP- of MPT-bestand) met de opgegeven instantie van de PrimaveraReadOptions-klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Beschrijving |
| --- | --- |
| projectTemplate | Pad naar sjabloon om project van te maken |
| options | de opgegeven instantie van de PrimaveraReadOptions-klasse. |

---

## Project (9 of 13) {#project_9}

Initialiseert een nieuw exemplaar van de Project-klasse om gegevens te lezen uit een database die is opgegeven door de instantie van de DbSettings-klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parameter | Beschrijving |
| --- | --- |
| instellingen | de opgegeven instantie van de DbSettings-klasse. |

---

## Project (10 of 13) {#project_10}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Beschrijving |
| --- | --- |
| stream | Stream om een sjabloon van te laden. |
| parseErrorHandler | de opgegeven callback-methode om xml-parsefouten af te handelen. |

---

## Project (11 of 13) {#project_11}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parameter | Beschrijving |
| --- | --- |
| stream | Stream om een sjabloon van te laden. |
| protectionPassword | Beschermingswachtwoord. |

---

## Project (12 of 13) {#project_12}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit een sjabloon (bestaand mpp- of mpt-bestand) met de opgegeven instantie van de LoadOptions-klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Beschrijving |
| --- | --- |
| projectTemplate | Pad naar sjabloon om project van te maken |
| options | de opgegeven instantie van de LoadOptions-klasse. |

---

## Project (13 of 13) {#project_13}

Initialiseert een nieuw exemplaar van de Project-klasse vanuit de Stream met de opgegeven instantie van de LoadOptions-klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Beschrijving |
| --- | --- |
| stream | Stream van de Project System::IO::Stream-klasse |
| options | de opgegeven instantie van de LoadOptions-klasse |

