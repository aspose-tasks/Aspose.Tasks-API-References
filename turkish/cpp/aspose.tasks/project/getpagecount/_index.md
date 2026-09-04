---
title: "Aspose::Tasks::Project::GetPageCount metodu"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "C++ için Aspose.Tasks"
description: "Varsayılan Timescale (Gün) kullanılarak render edilecek projenin sayfa sayısını döndürür."
type: docs
weight: 1090
url: /tr/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Varsayılan Timescale (Gün) kullanılarak render edilecek projenin sayfa sayısını döndürür.

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Verilen SaveOptions kullanılarak render edilecek proje için sayfa sayısını döndürür.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parametre | Açıklama |
| --- | --- |
| saveOptions | Sayfa sayısını almak için kaydetme seçenekleri. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Verilen Timescale ve PageSize kullanılarak render edilecek proje için sayfa sayısını döndürür.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parametre | Açıklama |
| --- | --- |
| pageSize | Sayfa sayısını almak için boyut. |
| scale | Sayfa sayısını almak için ölçek. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Verilen Timescale, PresentationFormat ve tarih aralığı kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parametre | Açıklama |
| --- | --- |
| pageSize | Sayfa sayısını almak için boyut. |
| scale | Sayfa sayısını almak için ölçek. |
| startDate | Sayfa sayısını almak için başlangıç tarihi. |
| endDate | Sayfa sayısını almak için bitiş tarihi. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Varsayılan Timescale (Gün) ve verilen PresentationFormat kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parametre | Açıklama |
| --- | --- |
| biçim | Sayfa sayısını almak için format. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Verilen Timescale ve PresentationFormat kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parametre | Açıklama |
| --- | --- |
| biçim | Sayfa sayısını almak için format. |
| scale | Sayfa sayısını almak için ölçek. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Verilen Timescale kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parametre | Açıklama |
| --- | --- |
| scale | Sayfa sayısını almak için ölçek. |

