---
title: "Aspose::Tasks::Project::GetPageCount méthode"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks pour C++"
description: "Renvoie le nombre de pages du projet à rendre en utilisant l'échelle de temps par défaut (Jours)."
type: docs
weight: 1090
url: /fr/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Renvoie le nombre de pages du projet à rendre en utilisant l'échelle de temps par défaut (Jours).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Renvoie le nombre de pages du projet à rendre en utilisant les SaveOptions fournis.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Paramètre | Description |
| --- | --- |
| saveOptions | Les options de sauvegarde pour obtenir le nombre de pages. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Renvoie le nombre de pages pour le projet à rendre en utilisant l'échelle de temps et la taille de page données.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Paramètre | Description |
| --- | --- |
| pageSize | La taille pour laquelle obtenir le nombre de pages. |
| scale | L'échelle pour laquelle obtenir le nombre de pages. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Renvoie le nombre de pages pour le projet à rendre en utilisant l'échelle de temps, le format de présentation et la plage de dates données.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Paramètre | Description |
| --- | --- |
| pageSize | La taille pour laquelle obtenir le nombre de pages. |
| scale | L'échelle pour laquelle obtenir le nombre de pages. |
| startDate | La date de début pour laquelle obtenir le nombre de pages. |
| endDate | La date de fin pour laquelle obtenir le nombre de pages. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Renvoie le nombre de pages pour le projet à rendre en utilisant l'échelle de temps par défaut (jours) et le format de présentation donné.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Paramètre | Description |
| --- | --- |
| format | Le format pour lequel obtenir le nombre de pages. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Renvoie le nombre de pages pour le projet à rendre en utilisant l'échelle de temps et le format de présentation donnés.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Paramètre | Description |
| --- | --- |
| format | Le format pour lequel obtenir le nombre de pages. |
| scale | L'échelle pour laquelle obtenir le nombre de pages. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Renvoie le nombre de pages pour le projet à rendre en utilisant l'échelle de temps donnée.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Paramètre | Description |
| --- | --- |
| scale | L'échelle pour laquelle obtenir le nombre de pages. |

