---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 870
url: /ja/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

指定された Project Online アカウントまたは<br/>            指定されたオンプレミスの Project Server インスタンス上のプロジェクトを読み取り、操作を実行するメソッドを提供するクラスです（Project Server のバージョン 2016 と 2019 がサポートされています）。

ProjectServerManager 型は次のメンバーを公開します:
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| ProjectServerManager(credentials) | [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/) クラスの新しいインスタンスを初期化します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| update_project(project) | 既定の保存オプションを使用して、Project Server\Project Online インスタンス内の既存プロジェクトを更新します。既存のプロジェクトは上書きされます。 |
| update_project(project, save_options) | 指定された保存オプションを使用して、Project Server\Project Online インスタンス内の既存プロジェクトを更新します。既存のプロジェクトは上書きされます。 |
| create_new_project(project) | 既定の保存オプションを使用して、Project Server\Project Online インスタンスに新しいプロジェクトを作成します。 |
| create_new_project(project, save_options) | 指定された保存オプションを使用して、Project Server\Project Online インスタンスに新しいプロジェクトを作成します。 |
| get_project(project_guid) | 指定された GUID のプロジェクトを Project Online アカウント \ Project Server インスタンスから取得します。 |
| get_project_raw_data(project_guid) | トラブルシューティングの目的でプロジェクトのバイナリデータを取得します。 |
| get_project_list() | 現在の Project Online アカウント \ Project Server インスタンスの「Working」ストアからプロジェクトのリストを取得します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

