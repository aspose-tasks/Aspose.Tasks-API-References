---
title: "SvgOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de projet vers SVG."
type: docs
weight: 283
url: /fr/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de projet vers SVG.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Initialise une nouvelle instance de la classe [SvgOptions](../../com.aspose.tasks/svgoptions) qui peut être utilisée pour enregistrer le projet au format SVG. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtient un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Définit un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Initialise une nouvelle instance de la classe [SvgOptions](../../com.aspose.tasks/svgoptions) qui peut être utilisée pour enregistrer le projet au format SVG.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Réservé à un usage interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Réservé à un usage interne.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtient un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.

--------------------

L'utilisation actuelle du pinceau dégradé n'est pas prise en charge pour le rendu en SVG.

**Returns:**
booléen - valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Définit un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet.

--------------------

L'utilisation actuelle du pinceau dégradé n'est pas prise en charge pour le rendu en SVG.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |

