---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GraphicalIndicatorCriteria कन्स्ट्रक्टर। GraphicalIndicatorCriteria टाइप का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

[`GraphicalIndicatorCriteria`](../) टाइप का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) एन्‍युम का मान जो दर्शाता है कि संकेतक किन पंक्तियों पर लागू होता है |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) का मान जो मानदंड द्वारा किए गए तुलना प्रकार को दर्शाता है। |
| imageIndex | Int32 | फ़ील्ड मानदंड को पूरा करने पर प्रदर्शित होने वाली इमेज का इंडेक्स |
| value1 | GraphicalIndicatorCriteriaValue | शर्त जाँच में उपयोग किए गए मान। |
| value2 | GraphicalIndicatorCriteriaValue | 'IsWithin' और 'IsNotWithing' स्थितियों के मामले में शर्त जाँच में उपयोग किया जाने वाला दूसरा मान (इंटरवल का अंत)। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | कन्स्ट्रक्टर को पास किए गए तर्कों के गलत संयोजन होने पर थ्रो किया जाता है। |

### संबंधित देखें

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

[`GraphicalIndicatorCriteria`](../) टाइप का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) एन्‍युम का मान जो दर्शाता है कि संकेतक किन पंक्तियों पर लागू होता है |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) का मान जो मानदंड द्वारा किए गए तुलना प्रकार को दर्शाता है। |
| imageIndex | Int32 | फ़ील्ड मानदंड को पूरा करने पर प्रदर्शित होने वाली इमेज का इंडेक्स |
| value | GraphicalIndicatorCriteriaValue | शर्त जाँच में उपयोग किया गया मान। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | कन्स्ट्रक्टर को पास किए गए तर्कों के गलत संयोजन होने पर थ्रो किया जाता है। |
| ArgumentException | जब IsWithin या IsNotWithing का मान परीक्षण तर्क में पास किया जाता है। |

### संबंधित देखें

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


