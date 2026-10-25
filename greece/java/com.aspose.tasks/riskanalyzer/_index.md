---
title: "RiskAnalyzer"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Πραγματοποιεί προσομοίωση Monte Carlo βασισμένη στις καθορισμένες ρυθμίσεις ανάλυσης κινδύνου."
type: docs
weight: 264
url: /el/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Πραγματοποιεί προσομοίωση Monte Carlo βασισμένη στις καθορισμένες ρυθμίσεις ανάλυσης κινδύνου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Πραγματοποιεί ανάλυση κινδύνου για το καθορισμένο έργο. |
| [getSettings()](#getSettings--) | Αποκτά το αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Ορίζει το αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | το καθορισμένο αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Πραγματοποιεί ανάλυση κινδύνου για το καθορισμένο έργο. Η ανάλυση βασίζεται στην προσομοίωση Monte Carlo και το αποτέλεσμα είναι ένα αντικείμενο της κλάσης [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | το καθορισμένο αντικείμενο της κλάσης [Project](../../com.aspose.tasks/project) για ανάλυση. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Αποκτά το αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Ορίζει το αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | το αντικείμενο της κλάσης [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου. |

