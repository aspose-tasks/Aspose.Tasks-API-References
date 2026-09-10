---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 980
url: /ja/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

プロジェクト内のリソース割り当てを表します。

ResourceAssignment 型は次のメンバーを公開します：
## プロパティ
| 名前 | 説明 |
| :- | :- |
| uid | Uid の値を取得または設定します。 |
| percent_work_complete | PercentWorkComplete の値を取得または設定します。 |
| actual_cost | ActualCost の値を取得または設定します。 |
| actual_finish | ActualFinish の値を取得または設定します。 |
| actual_overtime_cost | ActualOvertimeCost の値を取得または設定します。 |
| actual_start | ActualStart の値を取得または設定します。 |
| actual_work | ActualWork の値を取得または設定します。 |
| acwp | ACWP の値を取得または設定します。 |
| confirmed | Confirmed が設定されているかどうかを示す値を取得または設定します。 |
| cost | Cost の値を取得または設定します。 |
| cost_rate_table_type | CostRateTableType の値を取得または設定します。 |
| cost_variance | CostVariance の値を取得または設定します。 |
| cv | CV の値を取得または設定します。 |
| delay | Delay の値を取得または設定します。 |
| finish | Finish の値を取得または設定します。 |
| finish_variance | FinishVariance の値を取得または設定します。 |
| hyperlink | Hyperlink の値を取得または設定します。 |
| hyperlink_address | HyperlinkAddress の値を取得または設定します。 |
| hyperlink_sub_address | HyperlinkSubAddress の値を取得または設定します。 |
| work_variance | WorkVariance の値を取得または設定します。 |
| has_fixed_rate_units | HasFixedRateUnits が設定されているかどうかを示す値を取得または設定します。 |
| fixed_material | FixedMaterial が設定されているかどうかを示す値を取得または設定します。 |
| leveling_delay | LevelingDelay の値を取得または設定します。 |
| linked_fields | LinkedFields が設定されているかどうかを示す値を取得または設定します。 |
| milestone | Milestone が設定されているかどうかを示す値を取得または設定します。 |
| notes_text | RTF データから抽出されたノートのプレーンテキストを取得または設定します。 |
| notes_rtf | RTF 形式のテキストノートを取得または設定します。 |
| overallocated | Overallocated が設定されているかどうかを示す値を取得または設定します。 |
| overtime_cost | OvertimeCost の値を取得または設定します。 |
| overtime_work | OvertimeWork の値を取得または設定します。 |
| peak_units | PeakUnits の値を取得または設定します。 |
| regular_work | RegularWork の値を取得または設定します。 |
| remaining_cost | RemainingCost の値を取得または設定します。 |
| remaining_overtime_cost | RemainingOvertimeCost の値を取得または設定します。 |
| remaining_overtime_work | RemainingOvertimeWork の値を取得または設定します。 |
| remaining_work | RemainingWork の値を取得または設定します。 |
| response_pending | ResponsePending が設定されているかどうかを示す値を取得または設定します。 |
| start | Start の値を取得または設定します。 |
| stop | Stop の値を取得または設定します。 |
| resume | Resume の値を取得または設定します。 |
| start_variance | StartVariance の値を取得または設定します。 |
| summary | Summary が設定されているかどうかを示す値を取得または設定します。 |
| sv | SV の値を取得または設定します。 |
| units | Units の値を取得または設定します。 |
| update_needed | UpdateNeeded が設定されているかどうかを示す値を取得または設定します。 |
| vac | VAC の値を取得または設定します。 |
| work | Work の値を取得または設定します。 |
| work_contour | WorkContour の値を取得または設定します。 |
| bcws | BCWS の値を取得または設定します。 |
| bcwp | BCWP の値を取得または設定します。 |
| booking_type | BookingType の値を取得または設定します。 |
| actual_work_protected | ActualWorkProtected の値を取得または設定します。 |
| actual_overtime_work_protected | ActualOvertimeWorkProtected の値を取得または設定します。 |
| actual_overtime_work | ActualOvertimeWork の値を取得または設定します。 |
| created | Created の値を取得または設定します。 |
| assignment_owner | AssignmentOwner の値を取得または設定します。 |
| assignment_owner_guid | AssignmentOwnerGuid の値を取得または設定します。 |
| budget_cost | BudgetCost の値を取得または設定します。 |
| budget_work | BudgetWork の値を取得または設定します。 |
| rate_scale | RateScale の値を取得または設定します。 |
| task | リソースが割り当てられるタスクです。 |
| resource | タスクに割り当てられたリソースです。 |
| guid | この割り当ての一意の識別子を取得または設定します。 |
| parent_project | この割り当ての親プロジェクトを取得します。 |
| baselines | AssignmentBaselineCollection オブジェクトを取得します。<br/>            割り当てに関連付けられたベースライン値のコレクションです。 |
| extended_attributes | このオブジェクトの ExtendedAttributeCollection クラスのインスタンスを取得または設定します。 |
| timephased_data | [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) クラスのインスタンスを取得または設定し、[timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) クラスの要素を含みます。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | 指定された [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) の開始日と終了日の範囲内で、[timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) クラスのインスタンスを含む [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) クラスのインスタンスを返します。 |
| get_timephased_data(start, end) | 指定された [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) の開始日と終了日の範囲内で、[timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) クラスのインスタンスを含む [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) クラスのインスタンスを返します。 |
| get_timephased_work(start, end, timephased_data_type) | 指定された日時間隔に対する時間別作業量を取得します。 |
| get_timephased_work(start, end) | 指定された日時間隔に対する時間別作業量を取得します。 |
| delete() | プロジェクトの割り当てコレクションからリソース割り当てを削除します。 |
| equals(other) | このインスタンスが指定された [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/) クラスのインスタンスと等しいかどうかを示す値を返します。 |
| timephased_data_from_task_duration(calendar) | タスクの期間と予定開始日に基づいて時間別データのリストを生成します。 |
| make_t_ps(start, time, calendar, list, is_working, type) | 時間別データのリストを生成します。 |
| split_task(start, finish, calendar) | タスクを2つの部分に分割します。 |
| set_material_resource_units(units, rate_scale_type) | 可変材料消費を伴う材料リソースの割り当ての単位を設定します。<br/>            可変材料消費とは、割り当て期間が変わると使用される材料の量が比例して変化することを意味します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

