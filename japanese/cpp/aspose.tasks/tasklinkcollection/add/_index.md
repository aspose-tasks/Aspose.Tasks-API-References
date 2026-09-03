---
title: "Aspose::Tasks::TaskLinkCollection::Add メソッド"
linktitle: "追加"
articleTitle: "追加"
second_title: "Aspose.Tasks for C++"
description: "Finish-Start タスクリンクのインスタンスを返します。このインスタンスは TaskLinkCollection オブジェクトに追加されています。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Finish-Start タスクリンクのインスタンスを返します。このインスタンスは TaskLinkCollection オブジェクトに追加されています。

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| パラメーター | 説明 |
| --- | --- |
| pred | 前任タスク。 |
| succ | 後続タスク。 |

---

## Add (2 of 4) {#add_2}

TaskLinkCollection オブジェクトに追加された TaskLink のインスタンスを返します。

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| パラメーター | 説明 |
| --- | --- |
| pred | 前任タスク。 |
| succ | 後続タスク。 |
| linkType | リンクタイプ TaskLinkType |

---

## Add (3 of 4) {#add_3}

TaskLinkCollection オブジェクトに追加された TaskLink のインスタンスを返します。

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| パラメーター | 説明 |
| --- | --- |
| pred | 前任タスク。 |
| succ | 後続タスク。 |
| linkType | リンクタイプ TaskLinkType |
| lag | リンク遅延期間。 |

---

## Add (4 of 4) {#add_4}

これは ICollection の Add メソッドのスタブ実装で、NotSupportedException をスローするだけです。

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| パラメーター | 説明 |
| --- | --- |
| 項目 | 追加する項目です。 |

