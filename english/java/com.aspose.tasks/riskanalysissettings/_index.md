---
title: RiskAnalysisSettings
second_title: Aspose.Tasks for Java API Reference
description: Specifies settings for performing risk analysis.
type: docs
weight: 262
url: /java/com.aspose.tasks/riskanalysissettings/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisSettings
```

Specifies settings for performing risk analysis.
## Constructors

| Constructor | Description |
| --- | --- |
| [RiskAnalysisSettings()](#RiskAnalysisSettings--) | Initializes a new instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getIterationsCount()](#getIterationsCount--) | Gets the number of iterations to use in Monte Carlo simulation. |
| [getPatterns()](#getPatterns--) | Gets a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class. |
| [setIterationsCount(int value)](#setIterationsCount-int-) | Sets the number of iterations to use in Monte Carlo simulation. |
### RiskAnalysisSettings() {#RiskAnalysisSettings--}
```
public RiskAnalysisSettings()
```


Initializes a new instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class.

### getIterationsCount() {#getIterationsCount--}
```
public final int getIterationsCount()
```


Gets the number of iterations to use in Monte Carlo simulation. The default value is 100.

**Returns:**
int - the number of iterations to use in Monte Carlo simulation.
### getPatterns() {#getPatterns--}
```
public final RiskPatternCollection getPatterns()
```


Gets a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.

**Returns:**
[RiskPatternCollection](../../com.aspose.tasks/riskpatterncollection) - a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.
### setIterationsCount(int value) {#setIterationsCount-int-}
```
public final void setIterationsCount(int value)
```


Sets the number of iterations to use in Monte Carlo simulation. The default value is 100.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of iterations to use in Monte Carlo simulation. |

