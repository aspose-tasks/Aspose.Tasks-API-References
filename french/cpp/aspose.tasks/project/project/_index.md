---
title: "Aspose::Tasks::Project::Project constructeur"
linktitle: "Projet"
articleTitle: "Projet"
second_title: "Aspose.Tasks pour C++"
description: "Initialise une nouvelle instance de la classe Project."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Initialise une nouvelle instance de la classe Project.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Initialise une nouvelle instance de la classe Project à partir d’un modèle protégé par mot de passe (fichier mpp ou mpt existant).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Paramètre | Description |
| --- | --- |
| projectTemplate | Chemin vers le modèle à partir duquel créer le projet. |
| protectionPassword | Mot de passe de protection. |

---

## Project (3 of 13) {#project_3}

Initialise une nouvelle instance de la classe Project à partir d’un modèle (fichier mpp ou mpt existant).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Paramètre | Description |
| --- | --- |
| projectTemplate | Chemin vers le modèle à partir duquel créer le projet. |

---

## Project (4 of 13) {#project_4}

Initialise une nouvelle instance de la classe Project à partir du Stream avec l’instance spécifiée de la classe PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| stream | Stream de la classe Project System::IO::Stream |
| options | l’instance spécifiée de la classe PrimaveraReadOptions qui permet de personnaliser la lecture des formats Primavera (XER ou XML). |

---

## Project (5 of 13) {#project_5}

Initialise une nouvelle instance de la classe Project à partir d’un modèle (fichier mpp ou mpt existant).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Paramètre | Description |
| --- | --- |
| projectTemplate | Chemin vers le modèle à partir duquel créer le projet. |
| parseErrorHandler | la méthode de rappel spécifiée pour gérer les erreurs d’analyse XML. |

---

## Project (6 of 13) {#project_6}

Initialise une nouvelle instance de la classe Project à partir d’un stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Paramètre | Description |
| --- | --- |
| stream | Stream à partir duquel charger un modèle. |

---

## Project (7 of 13) {#project_7}

Initialise une nouvelle instance de la classe Project à partir d’une instance de StreamReader.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Paramètre | Description |
| --- | --- |
| reader | Le lecteur de flux où charger un modèle. |

---

## Project (8 of 13) {#project_8}

Initialise une nouvelle instance de la classe Project à partir d'un modèle (fichier MPP ou MPT existant) avec l'instance spécifiée de la classe PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| projectTemplate | Chemin vers le modèle à partir duquel créer le projet |
| options | l'instance spécifiée de la classe PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

Initialise une nouvelle instance de la classe Project pour lire les données d'une base de données spécifiée par l'instance de la classe DbSettings.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Paramètre | Description |
| --- | --- |
| paramètres | l'instance spécifiée de la classe DbSettings. |

---

## Project (10 of 13) {#project_10}

Initialise une nouvelle instance de la classe Project à partir d'un modèle (fichier mpp ou mpt existant).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Paramètre | Description |
| --- | --- |
| stream | Stream à partir duquel charger un modèle. |
| parseErrorHandler | la méthode de rappel spécifiée pour gérer les erreurs d’analyse XML. |

---

## Project (11 of 13) {#project_11}

Initialise une nouvelle instance de la classe Project à partir d'un modèle (fichier mpp ou mpt existant).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Paramètre | Description |
| --- | --- |
| stream | Stream à partir duquel charger un modèle. |
| protectionPassword | Mot de passe de protection. |

---

## Project (12 of 13) {#project_12}

Initialise une nouvelle instance de la classe Project à partir d'un modèle (fichier mpp ou mpt existant) avec l'instance spécifiée de la classe LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| projectTemplate | Chemin vers le modèle à partir duquel créer le projet |
| options | l'instance spécifiée de la classe LoadOptions. |

---

## Project (13 of 13) {#project_13}

Initialise une nouvelle instance de la classe Project à partir du flux avec l'instance spécifiée de la classe LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| stream | Stream de la classe Project System::IO::Stream |
| options | l'instance spécifiée de la classe LoadOptions |

