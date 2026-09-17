---
title: ProgressNotificationArgs
second_title: Aspose.Tasks for Java API Reference
description: Provides progress information for .
type: docs
weight: 220
url: /java/com.aspose.tasks/progressnotificationargs/
---

**Inheritance:**
java.lang.Object
```
public final class ProgressNotificationArgs
```

Provides progress information for [IProgressNotificationCallback.notify(ProgressNotificationArgs)](../../com.aspose.tasks/iprogressnotificationcallback\#notify-ProgressNotificationArgs-).
## Constructors

| Constructor | Description |
| --- | --- |
| [ProgressNotificationArgs()](#ProgressNotificationArgs--) | Initializes a new instance of the [ProgressNotificationArgs](../../com.aspose.tasks/progressnotificationargs) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCurrentStepName()](#getCurrentStepName--) | Gets the name of the current step (part of the operation) being executed. |
| [getCurrentStepProgress()](#getCurrentStepProgress--) | Gets the estimated progress percentage completed for the current step (part of the operation) (0-100). |
| [getEstimatedTotalProgress()](#getEstimatedTotalProgress--) | Gets the estimated total progress of the entire operation (0-100). |
### ProgressNotificationArgs() {#ProgressNotificationArgs--}
```
public ProgressNotificationArgs()
```


Initializes a new instance of the [ProgressNotificationArgs](../../com.aspose.tasks/progressnotificationargs) class.

### getCurrentStepName() {#getCurrentStepName--}
```
public String getCurrentStepName()
```


Gets the name of the current step (part of the operation) being executed.

**Returns:**
java.lang.String - the name of the current step (part of the operation) being executed.
### getCurrentStepProgress() {#getCurrentStepProgress--}
```
public int getCurrentStepProgress()
```


Gets the estimated progress percentage completed for the current step (part of the operation) (0-100).

**Returns:**
int - the estimated progress percentage completed for the current step (part of the operation) (0-100).
### getEstimatedTotalProgress() {#getEstimatedTotalProgress--}
```
public int getEstimatedTotalProgress()
```


Gets the estimated total progress of the entire operation (0-100).

**Returns:**
int - the estimated total progress of the entire operation (0-100).
