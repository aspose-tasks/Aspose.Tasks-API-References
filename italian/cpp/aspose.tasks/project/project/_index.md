---
title: "Aspose::Tasks::Project::Project costruttore"
linktitle: "Progetto"
articleTitle: "Progetto"
second_title: "Aspose.Tasks per C++"
description: "Inizializza una nuova istanza della classe Project."
type: docs
weight: 10
url: /it/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Inizializza una nuova istanza della classe Project.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Inizializza una nuova istanza della classe Project da un modello protetto da password (file mpp o mpt esistente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parametro | Descrizione |
| --- | --- |
| projectTemplate | Percorso del modello da cui creare il progetto. |
| protectionPassword | Password di protezione. |

---

## Project (3 of 13) {#project_3}

Inizializza una nuova istanza della classe Project da un modello (file mpp o mpt esistente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parametro | Descrizione |
| --- | --- |
| projectTemplate | Percorso del modello da cui creare il progetto. |

---

## Project (4 of 13) {#project_4}

Inizializza una nuova istanza della classe Project dallo Stream con la specifica istanza della classe PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parametro | Descrizione |
| --- | --- |
| stream | Stream della classe Project System::IO::Stream |
| options | l'istanza specificata della classe PrimaveraReadOptions che consente di personalizzare la lettura dei formati Primavera (XER o XML). |

---

## Project (5 of 13) {#project_5}

Inizializza una nuova istanza della classe Project da un modello (file mpp o mpt esistente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parametro | Descrizione |
| --- | --- |
| projectTemplate | Percorso del modello da cui creare il progetto. |
| parseErrorHandler | il metodo di callback specificato per gestire gli errori di parsing XML. |

---

## Project (6 of 13) {#project_6}

Inizializza una nuova istanza della classe Project da uno stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parametro | Descrizione |
| --- | --- |
| stream | Stream da cui caricare un modello. |

---

## Project (7 of 13) {#project_7}

Inizializza una nuova istanza della classe Project da un'istanza di StreamReader.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parametro | Descrizione |
| --- | --- |
| reader | Il lettore di flusso da cui caricare un modello. |

---

## Project (8 of 13) {#project_8}

Inizializza una nuova istanza della classe Project da un modello (file MPP o MPT esistente) con l'istanza specificata della classe PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parametro | Descrizione |
| --- | --- |
| projectTemplate | Percorso del modello da cui creare il progetto |
| options | l'istanza specificata della classe PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

Inizializza una nuova istanza della classe Project per leggere i dati da un database specificato dall'istanza della classe DbSettings.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parametro | Descrizione |
| --- | --- |
| impostazioni | l'istanza specificata della classe DbSettings. |

---

## Project (10 of 13) {#project_10}

Inizializza una nuova istanza della classe Project da un modello (file mpp o mpt esistente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parametro | Descrizione |
| --- | --- |
| stream | Stream da cui caricare un modello. |
| parseErrorHandler | il metodo di callback specificato per gestire gli errori di parsing XML. |

---

## Project (11 of 13) {#project_11}

Inizializza una nuova istanza della classe Project da un modello (file mpp o mpt esistente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parametro | Descrizione |
| --- | --- |
| stream | Stream da cui caricare un modello. |
| protectionPassword | Password di protezione. |

---

## Project (12 of 13) {#project_12}

Inizializza una nuova istanza della classe Project da un modello (file mpp o mpt esistente) con l'istanza specificata della classe LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parametro | Descrizione |
| --- | --- |
| projectTemplate | Percorso del modello da cui creare il progetto |
| options | l'istanza specificata della classe LoadOptions. |

---

## Project (13 of 13) {#project_13}

Inizializza una nuova istanza della classe Project dallo Stream con l'istanza specificata della classe LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parametro | Descrizione |
| --- | --- |
| stream | Stream della classe Project System::IO::Stream |
| options | l'istanza specificata della classe LoadOptions |

