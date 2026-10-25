---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "フィールドに対する便利な操作を提供するヘルパークラスです。"
type: docs
weight: 88
url: /ja/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

フィールドに対する便利な操作を提供するヘルパークラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | 特定のフィールドのデフォルトタイトルを返します。 |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | 特定のタスクフィールドのデフォルトタイトルを返します。 |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


特定のフィールドのデフォルトタイトルを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| フィールド | int | デフォルトタイトルを取得するフィールド。 |

**Returns:**
java.lang.String - 特定のフィールドが MS Project のビューに表示できる場合のデフォルトタイトル、そうでない場合は null。
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


特定のタスクフィールドのデフォルトタイトルを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| taskKey | バイト | デフォルトタイトルを取得するタスクフィールド。 |

**Returns:**
java.lang.String - 特定のタスクフィールドが MS Project のビューに表示できる場合のデフォルトタイトル、そうでない場合は null。
