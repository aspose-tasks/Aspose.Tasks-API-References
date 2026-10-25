---
title: "Constructor Aspose::Tasks::Project::Project"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks for C++"
description: "Inicializa una nueva instancia de la clase Project."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Inicializa una nueva instancia de la clase Project.

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

Inicializa una nueva instancia de la clase Project a partir de una plantilla protegida con contraseña (archivo mpp o mpt existente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| Parámetro | Descripción |
| --- | --- |
| projectTemplate | Ruta a la plantilla desde la cual crear el proyecto. |
| protectionPassword | Contraseña de protección. |

---

## Project (3 of 13) {#project_3}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo mpp o mpt existente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| Parámetro | Descripción |
| --- | --- |
| projectTemplate | Ruta a la plantilla desde la cual crear el proyecto. |

---

## Project (4 of 13) {#project_4}

Inicializa una nueva instancia de la clase Project a partir del Stream con la instancia especificada de la clase PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parámetro | Descripción |
| --- | --- |
| stream | Stream de la clase Project System::IO::Stream |
| options | la instancia especificada de la clase PrimaveraReadOptions que permite personalizar la lectura de formatos Primavera (XER o XML). |

---

## Project (5 of 13) {#project_5}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo mpp o mpt existente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parámetro | Descripción |
| --- | --- |
| projectTemplate | Ruta a la plantilla desde la cual crear el proyecto. |
| parseErrorHandler | el método de devolución de llamada especificado para manejar errores de análisis XML. |

---

## Project (6 of 13) {#project_6}

Inicializa una nueva instancia de la clase Project a partir de un stream.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parámetro | Descripción |
| --- | --- |
| stream | Stream desde el cual cargar una plantilla. |

---

## Project (7 of 13) {#project_7}

Inicializa una nueva instancia de la clase Project a partir de una instancia de StreamReader.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| Parámetro | Descripción |
| --- | --- |
| reader | El lector de flujo desde el cual cargar una plantilla. |

---

## Project (8 of 13) {#project_8}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo MPP o MPT existente) con la instancia especificada de la clase PrimaveraReadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| Parámetro | Descripción |
| --- | --- |
| projectTemplate | Ruta a la plantilla desde la cual crear el proyecto |
| options | la instancia especificada de la clase PrimaveraReadOptions. |

---

## Project (9 of 13) {#project_9}

Inicializa una nueva instancia de la clase Project para leer datos de una base de datos especificada por la instancia de la clase DbSettings.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| Parámetro | Descripción |
| --- | --- |
| configuración | la instancia especificada de la clase DbSettings. |

---

## Project (10 of 13) {#project_10}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo mpp o mpt existente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| Parámetro | Descripción |
| --- | --- |
| stream | Stream desde el cual cargar una plantilla. |
| parseErrorHandler | el método de devolución de llamada especificado para manejar errores de análisis XML. |

---

## Project (11 of 13) {#project_11}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo mpp o mpt existente).

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| Parámetro | Descripción |
| --- | --- |
| stream | Stream desde el cual cargar una plantilla. |
| protectionPassword | Contraseña de protección. |

---

## Project (12 of 13) {#project_12}

Inicializa una nueva instancia de la clase Project a partir de una plantilla (archivo mpp o mpt existente) con la instancia especificada de la clase LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| Parámetro | Descripción |
| --- | --- |
| projectTemplate | Ruta a la plantilla desde la cual crear el proyecto |
| options | la instancia especificada de la clase LoadOptions. |

---

## Project (13 of 13) {#project_13}

Inicializa una nueva instancia de la clase Project desde el Stream con la instancia especificada de la clase LoadOptions.

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| Parámetro | Descripción |
| --- | --- |
| stream | Stream de la clase Project System::IO::Stream |
| options | la instancia especificada de la clase LoadOptions |

