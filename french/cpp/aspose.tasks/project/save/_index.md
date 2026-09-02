---
title: "Aspose::Tasks::Project::Save méthode"
linktitle: "Save"
articleTitle: "Save"
second_title: "Aspose.Tasks pour C++"
description: "Enregistre le projet dans un flux en utilisant les options d'enregistrement spécifiées."
type: docs
weight: 1190
url: /fr/cpp/aspose.tasks/project/save/
---

## Save (1 of 5) {#save_1}

Enregistre le projet dans un flux en utilisant les options d'enregistrement spécifiées.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| stream | Le flux. |
| options | Les options d'enregistrement. |

---

## Save (2 of 5) {#save_2}

Enregistre les données du projet dans le flux.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, Saving::SaveFileFormat format)
```

| Paramètre | Description |
| --- | --- |
| stream | Le flux. |
| format | le format de fichier d'enregistrement spécifié. SaveFileFormat |

---

## Save (3 of 5) {#save_3}

Enregistre les données du projet dans le fichier au format mpp.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename)
```

| Paramètre | Description |
| --- | --- |
| nom de fichier | Le nom de fichier. |

---

## Save (4 of 5) {#save_4}

Enregistre le document dans un fichier en utilisant les options d'enregistrement spécifiées.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| Paramètre | Description |
| --- | --- |
| nom de fichier | Le nom de fichier. |
| options | Les options d'enregistrement. |

---

## Save (5 of 5) {#save_5}

Enregistre les données du projet dans le fichier.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, Saving::SaveFileFormat format)
```

| Paramètre | Description |
| --- | --- |
| nom de fichier | Le nom de fichier. |
| format | Le format de fichier d'enregistrement. |

