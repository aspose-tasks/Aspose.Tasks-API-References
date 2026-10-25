---
title: "Aspose::Tasks::Project::Project Konstruktor"
linktitle: "Projekt"
articleTitle: "Projekt"
second_title: "Aspose.Tasks für C++"
description: "Initialisiert eine neue Instanz der Project‑Klasse."
type: docs
weight: 10
url: /de/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Initialisiert eine neue Instanz der Project‑Klasse.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Initialisiert eine neue Instanz der Project-Klasse aus einer passwortgeschützten Vorlage (bestehende mpp- oder mpt-Datei).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parameter | Beschreibung |
| --- | --- |
| projectTemplate | Pfad zur Vorlage, aus der das Projekt erstellt wird. |
| protectionPassword | Schutzkennwort. |

---

## Project (3 of 13) {#project_3}

Initialisiert eine neue Instanz der Project-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parameter | Beschreibung |
| --- | --- |
| projectTemplate | Pfad zur Vorlage, aus der das Projekt erstellt wird. |

---

## Project (4 of 13) {#project_4}

Initialisiert eine neue Instanz der Project-Klasse aus dem Stream mit der angegebenen Instanz der PrimaveraReadOptions-Klasse.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Beschreibung |
| --- | --- |
| stream | Stream der Project System::IO::Stream Klasse |
| options | die angegebene Instanz der PrimaveraReadOptions-Klasse, die das Anpassen des Lesens von Primavera-Formaten (XER oder XML) ermöglicht. |

---

## Project (5 of 13) {#project_5}

Initialisiert eine neue Instanz der Project-Klasse aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parameter | Beschreibung |
| --- | --- |
| projectTemplate | Pfad zur Vorlage, aus der das Projekt erstellt wird. |
| parseErrorHandler | die angegebene Callback-Methode zur Behandlung von XML-Parsing-Fehlern. |

---

## Project (6 of 13) {#project_6}

Initialisiert eine neue Instanz der Project-Klasse aus einem Stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parameter | Beschreibung |
| --- | --- |
| stream | Stream, aus dem eine Vorlage geladen wird. |

---

## Project (7 of 13) {#project_7}

Initialisiert eine neue Instanz der Klasse Project aus einer StreamReader-Instanz.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parameter | Beschreibung |
| --- | --- |
| reader | Der StreamReader, aus dem eine Vorlage geladen werden soll. |

---

## Project (8 of 13) {#project_8}

Initialisiert eine neue Instanz der Klasse Project aus einer Vorlage (bestehende MPP- oder MPT-Datei) mit der angegebenen Instanz der Klasse PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parameter | Beschreibung |
| --- | --- |
| projectTemplate | Pfad zur Vorlage, aus der das Projekt erstellt wird |
| options | die angegebene Instanz der Klasse PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

Initialisiert eine neue Instanz der Klasse Project, um Daten aus einer Datenbank zu lesen, die durch die Instanz der Klasse DbSettings angegeben wird.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parameter | Beschreibung |
| --- | --- |
| settings | die angegebene Instanz der Klasse DbSettings. |

---

## Project (10 of 13) {#project_10}

Initialisiert eine neue Instanz der Klasse Project aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parameter | Beschreibung |
| --- | --- |
| stream | Stream, aus dem eine Vorlage geladen wird. |
| parseErrorHandler | die angegebene Callback-Methode zur Behandlung von XML-Parsing-Fehlern. |

---

## Project (11 of 13) {#project_11}

Initialisiert eine neue Instanz der Klasse Project aus einer Vorlage (bestehende mpp- oder mpt-Datei).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parameter | Beschreibung |
| --- | --- |
| stream | Stream, aus dem eine Vorlage geladen wird. |
| protectionPassword | Schutzkennwort. |

---

## Project (12 of 13) {#project_12}

Initialisiert eine neue Instanz der Klasse Project aus einer Vorlage (bestehende mpp- oder mpt-Datei) mit der angegebenen Instanz der Klasse LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Beschreibung |
| --- | --- |
| projectTemplate | Pfad zur Vorlage, aus der das Projekt erstellt wird |
| options | die angegebene Instanz der Klasse LoadOptions. |

---

## Project (13 of 13) {#project_13}

Initialisiert eine neue Instanz der Klasse Project aus dem Stream mit der angegebenen Instanz der Klasse LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parameter | Beschreibung |
| --- | --- |
| stream | Stream der Project System::IO::Stream Klasse |
| options | die angegebene Instanz der Klasse LoadOptions |

