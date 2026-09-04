---
title: "RiskAnalysisResult"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un résultat d'analyse de risque."
type: docs
weight: 262
url: /fr/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Représente un résultat d'analyse de risque.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Renvoie une instance de la [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) pour le type de risque spécifié. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Enregistre le rapport d'analyse des risques dans le flux au format PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Enregistre le rapport d'analyse des risques dans le chemin de fichier spécifié au format PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Renvoie une instance de la [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) pour le type de risque spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| itemType | int | le type de risque spécifié ; peut être l'une des valeurs de l'énumération [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Enregistre le rapport d'analyse des risques dans le flux au format PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux dans lequel enregistrer le rapport d'analyse des risques. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Enregistre le rapport d'analyse des risques dans le chemin de fichier spécifié au format PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom de fichier spécifié. |

