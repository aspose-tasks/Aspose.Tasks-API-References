---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GraphicalIndicatorCriteria yapıcı. GraphicalIndicatorCriteria tipinin yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

[`GraphicalIndicatorCriteria`](../) tipinin yeni bir örneğini başlatır.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum değeri, göstergenin hangi satırlara uygulandığını belirtir. |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) değeri, kriter tarafından gerçekleştirilen karşılaştırma türünü belirtir. |
| imageIndex | Int32 | alan kriteri karşıladığında görüntülenecek resmin indeksi |
| value1 | GraphicalIndicatorCriteriaValue | koşul kontrolünde kullanılan değerler. |
| value2 | GraphicalIndicatorCriteriaValue | İkinci değer (aralığın sonu), 'IsWithin' ve 'IsNotWithing' koşullarında koşul kontrolünde kullanılır. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | Yapıcıya hatalı bir argüman kombinasyonu geçirildiğinde fırlatılır. |

### Ayrıca Bakınız

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

[`GraphicalIndicatorCriteria`](../) tipinin yeni bir örneğini başlatır.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum değeri, göstergenin hangi satırlara uygulandığını belirtir. |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) değeri, kriter tarafından gerçekleştirilen karşılaştırma türünü belirtir. |
| imageIndex | Int32 | alan kriteri karşıladığında görüntülenecek resmin indeksi |
| value | GraphicalIndicatorCriteriaValue | koşul kontrolünde kullanılan değer. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | Yapıcıya hatalı bir argüman kombinasyonu geçirildiğinde fırlatılır. |
| ArgumentException | IsWithin ve IsNotWithing değerlerinden biri test argümanına geçirildiğinde. |

### Ayrıca Bakınız

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


