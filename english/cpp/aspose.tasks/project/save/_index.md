---
title: "Aspose::Tasks::Project::Save method"
linktitle: "Save"
articleTitle: "Save"
second_title: "Aspose.Tasks for C++"
description: "Saves the project to a stream using the specified save options."
type: docs
weight: 1190
url: /cpp/aspose.tasks/project/save/
---

## Save (1 of 5) {#save_1}

Saves the project to a stream using the specified save options.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| Parameter | Description |
| --- | --- |
| stream | The stream. |
| options | The save options. |

---

## Save (2 of 5) {#save_2}

Saves the project data to the stream.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, Saving::SaveFileFormat format)
```

| Parameter | Description |
| --- | --- |
| stream | The stream. |
| format | the specified save file format. SaveFileFormat |

---

## Save (3 of 5) {#save_3}

Saves the project data to the file in mpp format.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename)
```

| Parameter | Description |
| --- | --- |
| filename | The file name. |

---

## Save (4 of 5) {#save_4}

Saves the document to a file using the specified save options.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| Parameter | Description |
| --- | --- |
| filename | The file name. |
| options | The save options. |

---

## Save (5 of 5) {#save_5}

Saves the project data to the file.

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, Saving::SaveFileFormat format)
```

| Parameter | Description |
| --- | --- |
| filename | The file name. |
| format | The save file format. |

