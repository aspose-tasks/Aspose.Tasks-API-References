---
title: "プロジェクト"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトを表します。"
type: docs
weight: 220
url: /ja/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

プロジェクトを表します。

--------------------

Aspose.Tasks ライブラリの中心的なクラスである **Project** です。

サポートされているプロジェクト管理フォーマット（MPP、MPT、MPX、XML）のいずれかを読み取るために **Project** を使用できます。

サポートされているいずれかのフォーマットで既存のドキュメントを読み込むには、ファイル名またはストリームを **Project** のコンストラクタのいずれかに渡します。空のプロジェクトを作成するには、パラメータなしのコンストラクタを呼び出します。

プロジェクトを任意の [SaveFileFormat](../../com.aspose.tasks/savefileformat) フォーマットで保存するには、Save メソッドのオーバーロードのいずれかを使用します。Primavera: P6 XML、PM XER；Microsoft Excel: XLSX、XML；固定レイアウト: PDF；画像: JPEG、PNG、BMP、TIFF、SVG；テキスト: TXT；その他: HTML。

プロジェクトを印刷するには、[print()](../../com.aspose.tasks/project\#print--) メソッドのオーバーロードのいずれかを使用します。

**Project** は、`Aspose.Tasks.Project.Views`（[getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-))、`Aspose.Tasks.Project.BuiltInProps`（[getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-))、`Aspose.Tasks.Project.CustomProps`（[getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-))、および `Aspose.Tasks.Project.ExtendedAttributes`（[getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)) といったプロジェクト全体の情報を格納します。これらのオブジェクトのほとんどは、**Project** クラスの対応するプロパティを介してアクセスできます。

**Project** は、[Task](../../com.aspose.tasks/task)、[Resource](../../com.aspose.tasks/resource)、[ResourceAssignment](../../com.aspose.tasks/resourceassignment)、[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) および [Calendar](../../com.aspose.tasks/calendar) などの他のプロジェクトエンティティを操作するためのエントリーポイントを含むルートエンティティです。

**Project** のエンティティは、型付きコレクションを介してアクセスできます。例えば `Aspose.Tasks.Task.Children`（[Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-))、`Aspose.Tasks.Project.Resources`（[getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-))、`Aspose.Tasks.Project.ResourceAssignments`（[getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)) などです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [Project()](#Project--) | 新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | パスワードで保護されたテンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(String projectTemplate)](#Project-java.lang.String-) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | 指定された [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスのインスタンスを使用して、ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | 指定された [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスのインスタンスを使用して、テンプレート（既存の MPP または MPT ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | インスタンス [DbSettings](../../com.aspose.tasks/dbsettings) クラスで指定されたデータベースからデータを読み取るために、新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | 指定された [LoadOptions](../../com.aspose.tasks/loadoptions) クラスのインスタンスを使用して、テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | 指定された [LoadOptions](../../com.aspose.tasks/loadoptions) クラスのインスタンスを使用して、ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | このコンテナ内でプロパティがマッピングされている値を返します。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | このコンテナ内で指定されたプロパティを指定された値にマッピングします。 |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。 |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。 |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | ルートタスクを含むプロジェクトのすべてのタスクを再帰的に列挙します。 |
| [getActualsInSync()](#getActualsInSync--) | ActualsInSync が設定されているかどうかを示す値を取得します。 |
| [getAdminProject()](#getAdminProject--) | AdminProject が設定されているかどうかを示す値を取得します。 |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | AreEditableActualCosts が設定されているかどうかを示す値を取得します。 |
| [getAuthor()](#getAuthor--) | Author の値を取得します。 |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を取得します。 |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算すべきかどうかを取得します。 |
| [getAutolink()](#getAutolink--) | Autolink が設定されているかどうかを示す値を取得します。 |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | BaselineForEarnedValue の値を取得します。 |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | ベースラインの保存時刻を返します。 |
| [getBuiltInProps()](#getBuiltInProps--) | プロジェクトの組み込みプロパティコレクションを取得します。 |
| [getCalculationMode()](#getCalculationMode--) | プロジェクトの計算モードを取得します。 |
| [getCalendar()](#getCalendar--) | Calendar の値を取得します。 |
| [getCalendars()](#getCalendars--) | この Project インスタンスの [CalendarCollection](../../com.aspose.tasks/calendarcollection) オブジェクトを取得します。 |
| [getCategory()](#getCategory--) | Category の値を取得します。 |
| [getComments()](#getComments--) | Comments の値を取得します。 |
| [getCompany()](#getCompany--) | Company の値を取得します。 |
| [getCreationDate()](#getCreationDate--) | CreationDate の値を取得します。 |
| [getCriticalPath()](#getCriticalPath--) | このプロジェクトのクリティカル パスを構成するクリティカル タスクのリストを含むコレクションを取得します。 |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | MS Project では、総余裕時間がこの日数以下の場合、タスクはクリティカルと見なされます。 |
| [getCurrencyCode()](#getCurrencyCode--) | CurrencyCode の値を取得します。 |
| [getCurrencyDigits()](#getCurrencyDigits--) | CurrencyDigits の値を取得します。 |
| [getCurrencySymbol()](#getCurrencySymbol--) | CurrencySymbol の値を取得します。 |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | CurrencySymbolPosition の値を取得します。 |
| [getCurrentDate()](#getCurrentDate--) | CurrentDate の値を取得します。 |
| [getCustomDateFormat()](#getCustomDateFormat--) | CustomDateFormat の値を取得します。 |
| [getCustomProps()](#getCustomProps--) | プロジェクトのカスタム プロパティ コレクションを取得します。 |
| [getDateFormat()](#getDateFormat--) | DateFormat の値を取得します。 |
| [getDaysPerMonth()](#getDaysPerMonth--) | DaysPerMonth の値を取得します。 |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | DefaultFinishTime の値を取得します。 |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | DefaultFixedCostAccrual の値を取得します。 |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | DefaultOvertimeRate の値を取得します。 |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | DefaultStandardRate の値を取得します。 |
| [getDefaultStartTime()](#getDefaultStartTime--) | DefaultStartTime の値を取得します。 |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | DefaultTaskEVMethod の値を取得します。 |
| [getDefaultTaskType()](#getDefaultTaskType--) | DefaultTaskType の値を取得します。 |
| [getDefaultView()](#getDefaultView--) | プロジェクトのデフォルトビューを取得します。 |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) クラスのインスタンスを取得します。このクラスは、プロジェクトのデフォルトの週の稼働日と稼働時間のコレクションを表します。 |
| [getDisplayOptions()](#getDisplayOptions--) | [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) クラスのインスタンスを取得します。 |
| [getDuration(double val)](#getDuration-double-) | [Duration](../../com.aspose.tasks/duration) オブジェクトを取得します。指定された単位数と、プロジェクトの設定 [Prj.DURATION\\_FORMAT](../../com.aspose.tasks/prj\\#DURATION-FORMAT) で定義されたデフォルトの期間形式が適用されます。 |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | [Duration](../../com.aspose.tasks/duration) オブジェクトを取得します。指定された数の [TimeUnitType](../../com.aspose.tasks/timeunittype) 単位が使用されます。 |
| [getDurationFormat()](#getDurationFormat--) | DurationFormat の値を取得します。 |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | EarnedValueMethod の値を取得します。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | ExtendedAttributeDefinitionCollection オブジェクトを取得します。 |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | ExtendedCreationDate の値を取得します。 |
| [getFinishDate()](#getFinishDate--) | FinishDate の値を取得します。 |
| [getFiscalYearStart()](#getFiscalYearStart--) | FiscalYearStart が設定されているかどうかを示す値を取得します。 |
| [getFyStartDate()](#getFyStartDate--) | FyStartDate の値を取得します。 |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | プロジェクトのグローバリゼーション（言語固有）設定を取得します。 |
| [getGuid()](#getGuid--) | Guid の値を取得します。 |
| [getHonorConstraints()](#getHonorConstraints--) | HonorConstraints が設定されているかどうかを示す値を取得します。 |
| [getHyperlinkBase()](#getHyperlinkBase--) | HyperlinkBase の値を取得します。 |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | InsertedProjectsLikeSummary が設定されているかどうかを示す値を取得します。 |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を取得します。 |
| [getKeywords()](#getKeywords--) | Keywords の値を取得します。 |
| [getLastAuthor()](#getLastAuthor--) | LastAuthor の値を取得します。 |
| [getLastPrinted()](#getLastPrinted--) | LastPrinted の値を取得します。 |
| [getLastSaved()](#getLastSaved--) | LastSaved の値を取得します。 |
| [getManager()](#getManager--) | Manager の値を取得します。 |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | MicrosoftProjectServerURL が設定されているかどうかを示す値を取得します。 |
| [getMinutesPerDay()](#getMinutesPerDay--) | MinutesPerDay の値を取得します。 |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | MinutesPerWeek の値を取得します。 |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | MoveCompletedEndsBack が設定されているかどうかを示す値を取得します。 |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | MoveCompletedEndsForward が設定されているかどうかを示す値を取得します。 |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | MoveRemainingStartsBack が設定されているかどうかを示す値を取得します。 |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | MoveRemainingStartsForward が設定されているかどうかを示す値を取得します。 |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | MultipleCriticalPaths が設定されているかどうかを示す値を取得します。 |
| [getName()](#getName--) | Name の値を取得します。 |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | NewTaskStartDate の値を取得します。 |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | NewTasksAreManual が設定されているかどうかを示す値を取得します。 |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | NewTasksEffortDriven が設定されているかどうかを示す値を取得します。 |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | NewTasksEstimated が設定されているかどうかを示す値を取得します。 |
| [getOleObjects()](#getOleObjects--) | このプロジェクトファイルにリンクまたは埋め込まれている [OleObject](../../com.aspose/tasks/oleobject) クラスのインスタンスを含むコレクションを取得します。 |
| [getOutlineCodes()](#getOutlineCodes--) | OutlineCodeDefinitionCollection オブジェクトを取得します。 |
| [getPageCount()](#getPageCount--) | デフォルトの [Timescale](../../com.aspose.tasks/timescale)(Days) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | 指定された [SaveOptions](../../com.aspose.tasks/saveoptions) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | 指定された [Timescale](../../com.aspose.tasks/timescale) と [PresentationFormat](../../com.aspose.tasks/presentationformat) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | 指定された [Timescale](../../com.aspose.tasks/timescale) と [PageSize](../../com.aspose.tasks/pagesize) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | 指定された [Timescale](../../com.aspose.tasks/timescale)、[PresentationFormat](../../com.aspose.tasks/presentationformat) と日付範囲を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | デフォルトの [Timescale](../../com.aspose.tasks/timescale)(Days) と指定された [PresentationFormat](../../com.aspose.tasks/presentationformat) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | 指定された [Timescale](../../com.aspose.tasks/timescale) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | 指定されたタスクの前任タスクであるタスクリンクのコレクションを返します。 |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | Primavera ファイルから読み取ったプロジェクトの Primavera 固有プロパティを含むオブジェクトを取得します。 |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | ProjectExternallyEdited が設定されているかどうかを示す値を取得します。 |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | ストリームからプロジェクト ファイル情報を取得します。 |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | ファイルからプロジェクト ファイル情報を読み取ります。 |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | RemoveFileProperties が設定されているかどうかを示す値を取得します。 |
| [getResourceAssignments()](#getResourceAssignments--) | ResourceAssignmentCollection オブジェクトを取得します。 |
| [getResourceFilters()](#getResourceFilters--) | リソースベースのフィルタ定義をすべて取得します。 |
| [getResourceGroups()](#getResourceGroups--) | リソースベースのグループ定義をすべて取得します。 |
| [getResources()](#getResources--) | ResourceCollection オブジェクトを取得します。 |
| [getRevision()](#getRevision--) | Revision の値を取得します。 |
| [getRootTask()](#getRootTask--) | タスク ツリーのルートを取得します。 |
| [getSaveVersion()](#getSaveVersion--) | SaveVersion の値を取得します。 |
| [getScheduleFromStart()](#getScheduleFromStart--) | ScheduleFromStart が設定されているかどうかを示す値を取得します。 |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | ShowProjectSummaryTask が設定されているかどうかを示す値を取得します。 |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | SplitsInProgressTasks が設定されているかどうかを示す値を取得します。 |
| [getSpreadActualCost()](#getSpreadActualCost--) | SpreadActualCost が設定されているかどうかを示す値を取得します。 |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | SpreadPercentComplete が設定されているかどうかを示す値を取得します。 |
| [getStartDate()](#getStartDate--) | StartDate の値を取得します。 |
| [getStatusDate()](#getStatusDate--) | StatusDate の値を取得します。 |
| [getSubject()](#getSubject--) | Subject の値を取得します。 |
| [getTables()](#getTables--) | [Table](../../com.aspose.tasks/table) オブジェクトのリストを取得します。 |
| [getTaskFilters()](#getTaskFilters--) | タスクベースのフィルタ定義をすべて取得します。 |
| [getTaskGroups()](#getTaskGroups--) | タスクベースのグループ定義をすべて取得します。 |
| [getTaskLinks()](#getTaskLinks--) | [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) オブジェクトを取得します。 |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | TaskUpdatesResource が設定されているかどうかを示す値を取得します。 |
| [getTemplate()](#getTemplate--) | Template の値を取得します。 |
| [getTimescaleFinish()](#getTimescaleFinish--) | TimescaleFinish の値を取得します。 |
| [getTimescaleStart()](#getTimescaleStart--) | TimescaleStart の値を取得します。 |
| [getTitle()](#getTitle--) | Title の値を取得します。 |
| [getUid()](#getUid--) | Uid の値を取得します。 |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | UpdateManuallyScheduledTasksWhenEditingLinks が設定されているかどうかを示す値を取得します。 |
| [getVbaProject()](#getVbaProject--) | `VbaProject` のインスタンスを取得します（[getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) クラス。 |
| [getViews()](#getViews--) | [View](../../com.aspose.tasks/view) オブジェクトのリストを取得します。 |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | プロジェクトの WBS コード定義を取得します。 |
| [getWeekStartDay()](#getWeekStartDay--) | WeekStartDay の値を取得します。 |
| [getWork(double val)](#getWork-double-) | [Duration](../../com.aspose.tasks/duration) オブジェクトを、指定された `double` 値とデフォルトの作業形式で取得します。 |
| [getWorkFormat()](#getWorkFormat--) | WorkFormat の値を取得します。 |
| [print()](#print--) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定でプロジェクトをデフォルトプリンターに印刷します。 |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定とカスタム保存オプションでプロジェクトをデフォルトプリンターに印刷します。 |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定に従ってプロジェクトを印刷します。 |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定とカスタム保存オプションに従ってプロジェクトを印刷します。 |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定、カスタム保存オプション、および指定されたドキュメント名に従ってプロジェクトを印刷します。 |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定に従ってプロジェクトを印刷します。 |
| [print(String printerName)](#print-java.lang.String-) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定で指定されたプリンターにプロジェクトを印刷します。 |
| [recalculate()](#recalculate--) | すべてのプロジェクトタスクの ID、アウトラインレベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、余裕時間、作業およびコストフィールドを計算します。 |
| [recalculate(boolean validate)](#recalculate-boolean-) | オプションの検証を使用して、すべてのプロジェクトタスクの ID、アウトラインレベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、余裕時間、作業およびコストフィールドを計算します。 |
| [recalculateResourceFields()](#recalculateResourceFields--) | リソースの Id、開始日、終了日を再計算します。 |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | リソースの開始日と終了日を再計算します。 |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | プロジェクトのリソース割り当てリストから無効なリソース割り当てを除外します。 |
| [renumberWBSCode()](#renumberWBSCode--) | すべてのタスクの WBS コードを再番号付けします。 |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | 渡されたタスクの WBS コードを再番号付けします。 |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | 未完了のプロジェクト作業を、指定された日付以降に開始するように再スケジュールします。 |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | 指定された日付以降に開始するよう、指定されたタスクのリストの未完了作業のスケジュールを変更します。 |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | 指定された保存オプションを使用して、プロジェクトをストリームに保存します。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | プロジェクトデータをストリームに保存します。 |
| [save(String filename)](#save-java.lang.String-) | プロジェクトデータを mpp 形式のファイルに保存します。 |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | 指定された保存オプションを使用して、ドキュメントをファイルに保存します。 |
| [save(String filename, int format)](#save-java.lang.String-int-) | プロジェクトデータをファイルに保存します。 |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | プロジェクトをテンプレートとして指定されたストリームに保存します。 |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | プロジェクトをテンプレートとして指定されたストリームに保存します。 |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | プロジェクトをテンプレートとして指定されたファイルパスに保存します。 |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | プロジェクトをテンプレートとして保存します。 |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | プロジェクト概要レポートをストリームに保存します。 |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | 指定されたタイプのプロジェクトレポートを指定されたストリームに保存します。 |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | プロジェクト概要レポートを PDF ファイルに保存します。 |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | 指定されたタイプのプロジェクトレポートを PDF 形式で指定されたファイルパスに保存します。 |
| [selectAllChildTasks()](#selectAllChildTasks--) | ルートタスクのすべての子タスクを再帰的に収集します。 |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | このコンテナ内で指定されたプロパティを指定された値にマッピングします。 |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | ActualsInSync が設定されているかどうかを示す値を設定します。 |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | AdminProject が設定されているかどうかを示す値を設定します。 |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | AreEditableActualCosts が設定されているかどうかを示す値を設定します。 |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Author の値を設定します。 |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を設定します。 |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動計算するかどうかを設定します。 |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | Autolink が設定されているかどうかを示す値を設定します。 |
| [setBaseline(int baselineType)](#setBaseline-int-) | プロジェクト全体の指定されたベースラインにベースラインフィールドを保存します。 |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | 選択されたタスクの指定されたベースラインにベースラインフィールドを保存します。 |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | BaselineForEarnedValue の値を設定します。 |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | ベースラインの保存時刻を設定します。 |
| [setCalculationMode(int value)](#setCalculationMode-int-) | プロジェクトの計算モードを設定します。 |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar の値を設定します。 |
| [setCategory(String value)](#setCategory-java.lang.String-) | カテゴリの値を設定します。 |
| [setComments(String value)](#setComments-java.lang.String-) | コメントの値を設定します。 |
| [setCompany(String value)](#setCompany-java.lang.String-) | 会社の値を設定します。 |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | CreationDate の値を設定します。 |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | MS Project では、総余裕時間がこの日数以下の場合、タスクはクリティカルと見なされます。 |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | CurrencyCode の値を設定します。 |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | CurrencyDigits の値を設定します。 |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | CurrencySymbol の値を設定します。 |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | CurrencySymbolPosition の値を設定します。 |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | CurrentDate の値を設定します。 |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | CustomDateFormat の値を設定します。 |
| [setDateFormat(int value)](#setDateFormat-int-) | DateFormat の値を設定します。 |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | DaysPerMonth の値を設定します。 |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | DefaultFinishTime の値を設定します。 |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | DefaultFixedCostAccrual の値を設定します。 |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | DefaultOvertimeRate の値を設定します。 |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | DefaultStandardRate の値を設定します。 |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | DefaultStartTime の値を設定します。 |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | DefaultTaskEVMethod の値を設定します。 |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | DefaultTaskType の値を設定します。 |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | プロジェクトのデフォルトビューを設定します。 |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | DurationFormat の値を設定します。 |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | EarnedValueMethod の値を設定します。 |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | ExtendedCreationDate の値を設定します。 |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | FinishDate の値を設定します。 |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | FiscalYearStart が設定されているかどうかを示す値を設定します。 |
| [setFyStartDate(int value)](#setFyStartDate-int-) | FyStartDate の値を設定します。 |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | プロジェクトのグローバリゼーション（言語固有）設定を設定します。 |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Guid の値を設定します。 |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | HonorConstraints が設定されているかどうかを示す値を設定します。 |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | HyperlinkBase の値を設定します。 |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | InsertedProjectsLikeSummary が設定されているかどうかを示す値を設定します。 |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を設定します。 |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Keywords の値を設定します。 |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | LastAuthor の値を設定します。 |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | LastPrinted の値を設定します。 |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | LastSaved の値を設定します。 |
| [setManager(String value)](#setManager-java.lang.String-) | Manager の値を設定します。 |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | MicrosoftProjectServerURL が設定されているかどうかを示す値を設定します。 |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | MinutesPerDay の値を設定します。 |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | MinutesPerWeek の値を設定します。 |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | MoveCompletedEndsBack が設定されているかどうかを示す値を設定します。 |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | MoveCompletedEndsForward が設定されているかどうかを示す値を設定します。 |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | MoveRemainingStartsBack が設定されているかどうかを示す値を設定します。 |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | MoveRemainingStartsForward が設定されているかどうかを示す値を設定します。 |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | MultipleCriticalPaths が設定されているかどうかを示す値を設定します。 |
| [setName(String value)](#setName-java.lang.String-) | Name の値を設定します。 |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | NewTaskStartDate の値を設定します。 |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | NewTasksAreManual が設定されているかどうかを示す値を設定します。 |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | NewTasksEffortDriven が設定されているかどうかを示す値を設定します。 |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | NewTasksEstimated が設定されているかどうかを示す値を設定します。 |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | ProjectExternallyEdited が設定されているかどうかを示す値を設定します。 |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | RemoveFileProperties が設定されているかどうかを示す値を設定します。 |
| [setRevision(int value)](#setRevision-int-) | Revision の値を設定します。 |
| [setSaveVersion(int value)](#setSaveVersion-int-) | SaveVersion の値を設定します。 |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | ScheduleFromStart が設定されているかどうかを示す値を設定します。 |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | ShowProjectSummaryTask が設定されているかどうかを示す値を設定します。 |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | SplitsInProgressTasks が設定されているかどうかを示す値を設定します。 |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | SpreadActualCost が設定されているかどうかを示す値を設定します。 |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | SpreadPercentComplete が設定されているかどうかを示す値を設定します。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | StartDate の値を設定します。 |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | StatusDate の値を設定します。 |
| [setSubject(String value)](#setSubject-java.lang.String-) | Subject の値を設定します。 |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | TaskUpdatesResource が設定されているかどうかを示す値を設定します。 |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Template の値を設定します。 |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | TimescaleFinish の値を設定します。 |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | TimescaleStart の値を設定します。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | Title の値を設定します。 |
| [setUid(String value)](#setUid-java.lang.String-) | Uid の値を設定します。 |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | UpdateManuallyScheduledTasksWhenEditingLinks が設定されているかどうかを示す値を設定します。 |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | プロジェクトの WBS コード定義を設定します。 |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | WeekStartDay の値を設定します。 |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | WorkFormat の値を設定します。 |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | プロジェクト全体の指定された日付までのすべての作業を完了として更新します。 |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | 指定されたタスクのリストに対して、指定された日付までのすべての作業を完了として更新します。 |
### Project() {#Project--}
```
public Project()
```


新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


パスワードで保護されたテンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectTemplate | java.lang.String | プロジェクト作成に使用するテンプレートへのパス。 |
|  | protectionPassword | java.lang.String | 保護パスワード。 |

--------------------

現在、MSP 2003 ファイル形式のみでパスワードで保護されたファイルの読み取りがサポートされています。 |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectTemplate | java.lang.String | プロジェクト作成に使用するテンプレートへのパス。 |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


指定された [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスのインスタンスを使用して、ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | プロジェクトのストリーム java.io.InputStream クラス |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Primavera のフォーマット (XER または XML) の読み取りをカスタマイズできる、[PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) クラスの指定されたインスタンス。 |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectTemplate | java.lang.String | プロジェクト作成に使用するテンプレートへのパス。 |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML パースエラーを処理するための、指定されたコールバック メソッド。 |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | テンプレートを読み込むための java.io.InputStream。 |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


指定された [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) クラスのインスタンスを使用して、テンプレート（既存の MPP または MPT ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectTemplate | java.lang.String | プロジェクト作成に使用するテンプレートへのパス |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) クラスの指定されたインスタンス。 |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


インスタンス [DbSettings](../../com.aspose.tasks/dbsettings) クラスで指定されたデータベースからデータを読み取るために、新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | [DbSettings](../../com.aspose/tasks/dbsettings) クラスの指定されたインスタンス。 |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | テンプレートを読み込むための java.io.InputStream。 |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | XML パースエラーを処理するための、指定されたコールバック メソッド。 |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | テンプレートを読み込むための java.io.InputStream。 |
|  | protectionPassword | java.lang.String | 保護パスワード。 |

--------------------

現在、MSP 2003 ファイル形式のみでパスワードで保護されたファイルの読み取りがサポートされています。 |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


指定された [LoadOptions](../../com.aspose.tasks/loadoptions) クラスのインスタンスを使用して、テンプレート（既存の mpp または mpt ファイル）から新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectTemplate | java.lang.String | プロジェクト作成に使用するテンプレートへのパス |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | [LoadOptions](../../com.aspose/tasks/loadoptions) クラスの指定されたインスタンス。 |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


指定された [LoadOptions](../../com.aspose.tasks/loadoptions) クラスのインスタンスを使用して、ストリームから新しい [Project](../../com.aspose.tasks/project) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | プロジェクトのストリーム java.io.InputStream クラス |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | [LoadOptions](../../com.aspose/tasks/loadoptions) クラスの指定されたインスタンス |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


このコンテナ内でプロパティがマッピングされている値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティ キー。[Prj](../../com.aspose.tasks/prj) はプロパティ キーを取得するために使用します。 |

**Returns:**
T - このコンテナ内でプロパティがマッピングされる値です。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


このコンテナ内で指定されたプロパティを指定された値にマッピングします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定されたプロパティ キー。[Prj](../../com.aspose.tasks/prj) はプロパティ キーを取得するために使用します。 |
| val | T | 値です。 |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | データをコピーする先の別のプロジェクト。 |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | データをコピーする先の別のプロジェクト。 |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | コピー処理を制御するコピー オプション。 |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


ルートタスクを含むプロジェクトのすべてのタスクを再帰的に列挙します。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - プロジェクトのすべてのタスクを反復処理できる IEnumerable。

--------------------

[selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) メソッドと比較して、すべてのタスクのメモリを割り当てずにタスクを反復処理できる、より軽量な方法を提供します。
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


ActualsInSync が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


AdminProject が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


AreEditableActualCosts が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


Author の値を取得します。

**Returns:**
java.lang.String - Author の値。
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算すべきかどうかを取得します。

**Returns:**
boolean - 割り当ての作業とリソースレートを使用して、割り当てコストと残存コストを自動的に計算すべきかどうか。
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


Autolink が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


BaselineForEarnedValue の値を取得します。

**Returns:**
int - BaselineForEarnedValue の値。
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


ベースラインの保存時刻を返します。ベースラインが保存されていない場合は DateTime.MinValue (00:00:00.0000000 UTC, 0001年1月1日) を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| baselineNumber | int | ベースラインの番号 [BaselineType](../../com.aspose.tasks/baselinetype)。 |

**Returns:**
java.util.Date - ベースラインの最終保存日時。
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


プロジェクトの組み込みプロパティコレクションを取得します。

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


プロジェクトの計算モードを取得します。`CalculationMode` 列挙体の値のいずれかです（[getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)）。

**Returns:**
int - プロジェクトの計算モード。
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar の値を取得します。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


この Project インスタンスの [CalendarCollection](../../com.aspose.tasks/calendarcollection) オブジェクトを取得します。

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


Category の値を取得します。

**Returns:**
java.lang.String - カテゴリの値。
### getComments() {#getComments--}
```
public final String getComments()
```


Comments の値を取得します。

**Returns:**
java.lang.String - コメントの値。
### getCompany() {#getCompany--}
```
public final String getCompany()
```


Company の値を取得します。

**Returns:**
java.lang.String - 会社の値。
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


CreationDate の値を取得します。

**Returns:**
java.util.Date - 作成日付の値。
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


このプロジェクトのクリティカル パスを構成するクリティカル タスクのリストを含むコレクションを取得します。

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

これは O(n) 操作で、n はプロジェクト内のタスク数です。
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


MS Project では、総余裕時間がこの日数以下の場合、タスクはクリティカルと見なされます。

**Returns:**
int - タスクがクリティカルとみなされる総余裕時間（日）の最大値。
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


CurrencyCode の値を取得します。

**Returns:**
java.lang.String - 通貨コードの値。
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


CurrencyDigits の値を取得します。

**Returns:**
int - 通貨桁数の値。
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


CurrencySymbol の値を取得します。

**Returns:**
java.lang.String - 通貨記号の値。
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


CurrencySymbolPosition の値を取得します。

**Returns:**
int - 通貨記号位置の値。
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


CurrentDate の値を取得します。

**Returns:**
java.util.Date - 現在日付の値。
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


CustomDateFormat の値を取得します。

**Returns:**
java.lang.String - カスタム日付形式の値。
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


プロジェクトのカスタム プロパティ コレクションを取得します。

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


DateFormat の値を取得します。

**Returns:**
int - 日付形式の値。
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


DaysPerMonth の値を取得します。

**Returns:**
int - 月あたりの日数の値。
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


DefaultFinishTime の値を取得します。

**Returns:**
java.util.Date - デフォルト終了時間の値。
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


DefaultFixedCostAccrual の値を取得します。

**Returns:**
int - デフォルト固定コスト累積の値。
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


DefaultOvertimeRate の値を取得します。

**Returns:**
double - デフォルト残業率の値。
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


DefaultStandardRate の値を取得します。

**Returns:**
double - デフォルト標準率の値。
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


DefaultStartTime の値を取得します。

**Returns:**
java.util.Date - デフォルト開始時間の値。
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


DefaultTaskEVMethod の値を取得します。

**Returns:**
int - デフォルトタスクEVメソッドの値。
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


DefaultTaskType の値を取得します。

**Returns:**
int - デフォルトタスクタイプの値。
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


プロジェクトのデフォルトビューを取得します。

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) クラスのインスタンスを取得します。このクラスは、プロジェクトのデフォルトの週の稼働日と稼働時間のコレクションを表します。

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

データは mpp ファイルのみに含まれ、xml には含まれません。
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) クラスのインスタンスを取得します。

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


[Duration](../../com.aspose.tasks/duration) オブジェクトを取得します。指定された単位数と、プロジェクトの設定 [Prj.DURATION\\_FORMAT](../../com.aspose.tasks/prj\\#DURATION-FORMAT) で定義されたデフォルトの期間形式が適用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | val | double | 指定された単位数。 |

--------------------

このメソッドは、Project.DurationFormat 設定に応じて異なる期間を返すため、注意して使用すべきです。たとえば、Project.DurationFormat が TimeUnitType.Hour の場合、GetWork(1.0) は 1 時間を返し、TimeUnitType.Day の場合は 1 日を返します。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


[Duration](../../com.aspose.tasks/duration) オブジェクトを取得します。指定された数の [TimeUnitType](../../com.aspose.tasks/timeunittype) 単位が使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| val | double | 指定された単位数。 |
| timeUnit | バイト | 指定された TimeUnitType の値。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


DurationFormat の値を取得します。

**Returns:**
byte - DurationFormat の値。
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


EarnedValueMethod の値を取得します。

**Returns:**
int - EarnedValueMethod の値。
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


ExtendedAttributeDefinitionCollection オブジェクトを取得します。プロジェクトに関連付けられた拡張属性（カスタム フィールド）定義のコレクションです。

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


ExtendedCreationDate の値を取得します。

**Returns:**
java.util.Date - ExtendedCreationDate の値。
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


FinishDate の値を取得します。

**Returns:**
java.util.Date - FinishDate の値。
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


FiscalYearStart が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


FyStartDate の値を取得します。

**Returns:**
int - FyStartDate の値。
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


プロジェクトのグローバリゼーション（言語固有）設定を取得します。

推奨される方法は、プロジェクト全体でカルチャに依存しないリテラルまたはフォーマットを使用することです。ただし、プロジェクトがカルチャ固有のリテラルを使用する場合、このクラスを使用して計算エンジンがそれらのリテラルを解析できるようにすることができます。

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Guid の値を取得します。

**Returns:**
java.util.UUID - Guid の値。
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


HonorConstraints が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


HyperlinkBase の値を取得します。

**Returns:**
java.lang.String - HyperlinkBase の値。
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


InsertedProjectsLikeSummary が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


Keywords の値を取得します。

**Returns:**
java.lang.String - Keywords の値。
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


LastAuthor の値を取得します。

**Returns:**
java.lang.String - LastAuthor の値。
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


LastPrinted の値を取得します。

**Returns:**
java.util.Date - LastPrinted の値。
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


LastSaved の値を取得します。

**Returns:**
java.util.Date - LastSaved の値。
### getManager() {#getManager--}
```
public final String getManager()
```


Manager の値を取得します。

**Returns:**
java.lang.String - Manager の値。
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


MicrosoftProjectServerURL が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


MinutesPerDay の値を取得します。

**Returns:**
int - MinutesPerDay の値。
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


MinutesPerWeek の値を取得します。

**Returns:**
int - MinutesPerWeek の値。
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


MoveCompletedEndsBack が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


MoveCompletedEndsForward が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


MoveRemainingStartsBack が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


MoveRemainingStartsForward が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


MultipleCriticalPaths が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


Name の値を取得します。

**Returns:**
java.lang.String - Name の値。
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


NewTaskStartDate の値を取得します。

**Returns:**
int - NewTaskStartDate の値。
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


NewTasksAreManual が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


NewTasksEffortDriven が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


NewTasksEstimated が設定されているかどうかを示す値を取得します。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


このプロジェクトファイルにリンクまたは埋め込まれている [OleObject](../../com.aspose/tasks/oleobject) クラスのインスタンスを含むコレクションを取得します。

--------------------

mpp ファイル形式のみで利用可能です。このコレクションは 'Clear' 操作を除き読み取り専用です。

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


OutlineCodeDefinitionCollection オブジェクトを取得します。プロジェクトに関連付けられたアウトライン コード定義のコレクションです。

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


デフォルトの [Timescale](../../com.aspose.tasks/timescale)(Days) を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:**
int - レンダリングされるページ数。
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


指定された [SaveOptions](../../com.aspose.tasks/saveoptions) を使用してレンダリングされるプロジェクトのページ数を返します。

--------------------

&gt; ```
&gt; この例では、HtmlSaveOptions のインスタンスと、生成された HTML のページ数がコンソールに出力されます。
&gt; ``````

  [C#]
Project project = new Project(@\"test.mpp\");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
public final int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
public final NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
public final boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
public final NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
public final NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
public final NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
public final Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
public final String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
public final NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
public final String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
public final Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
public final Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
public final String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
public final String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
public final NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
public final int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

