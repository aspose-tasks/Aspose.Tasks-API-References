---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor GraphicalIndicatorCriteria. Menginisialisasi sebuah instance baru dari tipe GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /id/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Menginisialisasi sebuah instance baru dari tipe [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | nilai dari enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) yang menunjukkan untuk baris mana indikator diterapkan |
| test | FilterComparisonType | nilai dari [`FilterComparisonType`](../../filtercomparisontype/) yang menunjukkan tipe perbandingan yang dilakukan oleh kriteria. |
| imageIndex | Int32 | indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria |
| value1 | GraphicalIndicatorCriteriaValue | nilai yang digunakan dalam pemeriksaan kondisi. |
| value2 | GraphicalIndicatorCriteriaValue | nilai kedua (akhir interval) yang digunakan dalam pemeriksaan kondisi dalam kasus kondisi 'IsWithin' dan 'IsNotWithing'. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Dilemparkan ketika kombinasi argumen yang tidak tepat diberikan ke konstruktor. |

### Lihat Juga

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Menginisialisasi sebuah instance baru dari tipe [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | nilai dari enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) yang menunjukkan untuk baris mana indikator diterapkan |
| test | FilterComparisonType | nilai dari [`FilterComparisonType`](../../filtercomparisontype/) yang menunjukkan tipe perbandingan yang dilakukan oleh kriteria. |
| imageIndex | Int32 | indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria |
| value | GraphicalIndicatorCriteriaValue | nilai yang digunakan dalam pemeriksaan kondisi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Dilemparkan ketika kombinasi argumen yang tidak tepat diberikan ke konstruktor. |
| ArgumentException | Ketika nilai IsWithin atau IsNotWithing diberikan ke argumen pengujian. |

### Lihat Juga

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


