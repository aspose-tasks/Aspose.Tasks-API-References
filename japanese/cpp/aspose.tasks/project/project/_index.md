---
title: "Aspose::Tasks::Project::Project コンストラクタ"
linktitle: "プロジェクト"
articleTitle: "プロジェクト"
second_title: "Aspose.Tasks for C++"
description: "Project クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

パスワードで保護されたテンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| パラメーター | 説明 |
| --- | --- |
| projectTemplate | プロジェクト作成に使用するテンプレートへのパス。 |
| protectionPassword | 保護パスワード。 |

---

## Project (3 of 13) {#project_3}

テンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| パラメーター | 説明 |
| --- | --- |
| projectTemplate | プロジェクト作成に使用するテンプレートへのパス。 |

---

## Project (4 of 13) {#project_4}

指定された PrimaveraReadOptions クラスのインスタンスと共にストリームから Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| stream | Project System::IO::Stream クラスのストリーム |
| options | PrimaveraReadOptions クラスの指定されたインスタンスで、Primavera フォーマット（XER または XML）の読み取りをカスタマイズできます。 |

---

## Project (5 of 13) {#project_5}

テンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| パラメーター | 説明 |
| --- | --- |
| projectTemplate | プロジェクト作成に使用するテンプレートへのパス。 |
| parseErrorHandler | XML パースエラーを処理するための指定されたコールバックメソッド。 |

---

## Project (6 of 13) {#project_6}

ストリームから Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| パラメーター | 説明 |
| --- | --- |
| stream | テンプレートを読み込むためのストリーム。 |

---

## Project (7 of 13) {#project_7}

StreamReader インスタンスから Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| パラメーター | 説明 |
| --- | --- |
| reader | テンプレートを読み込むストリームリーダー。 |

---

## Project (8 of 13) {#project_8}

指定された PrimaveraReadOptions クラスのインスタンスを使用して、テンプレート（既存の MPP または MPT ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| projectTemplate | プロジェクトを作成するテンプレートへのパス |
| options | 指定された PrimaveraReadOptions クラスのインスタンス。 |

---

## Project (9 of 13) {#project_9}

DbSettings クラスのインスタンスで指定されたデータベースからデータを読み取るために、Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| パラメーター | 説明 |
| --- | --- |
| 設定 | 指定された DbSettings クラスのインスタンス。 |

---

## Project (10 of 13) {#project_10}

テンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| パラメーター | 説明 |
| --- | --- |
| stream | テンプレートを読み込むためのストリーム。 |
| parseErrorHandler | XML パースエラーを処理するための指定されたコールバックメソッド。 |

---

## Project (11 of 13) {#project_11}

テンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| パラメーター | 説明 |
| --- | --- |
| stream | テンプレートを読み込むためのストリーム。 |
| protectionPassword | 保護パスワード。 |

---

## Project (12 of 13) {#project_12}

指定された LoadOptions クラスのインスタンスを使用して、テンプレート（既存の mpp または mpt ファイル）から Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| projectTemplate | プロジェクトを作成するテンプレートへのパス |
| options | 指定された LoadOptions クラスのインスタンス。 |

---

## Project (13 of 13) {#project_13}

指定された LoadOptions クラスのインスタンスを使用して、ストリームから Project クラスの新しいインスタンスを初期化します。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| stream | Project System::IO::Stream クラスのストリーム |
| options | 指定された LoadOptions クラスのインスタンス |

