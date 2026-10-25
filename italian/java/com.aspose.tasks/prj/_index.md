---
title: "Prj"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta le proprietà supportate dell'oggetto."
type: docs
weight: 216
url: /it/java/com.aspose.tasks/prj/
---

**Inheritance:**
java.lang.Object
```
public class Prj
```

Rappresenta le proprietà supportate dell'oggetto [Project](../../com.aspose.tasks/project).
## Campi

| Campo | Descrizione |
| --- | --- |
| [ACTUALS_IN_SYNC](#ACTUALS-IN-SYNC) | Determina se tutti i lavori effettivi sono stati sincronizzati con il progetto. |
| [ADMIN_PROJECT](#ADMIN-PROJECT) | Determina se un progetto è un progetto amministrativo. |
| [ARE_EDITABLE_ACTUAL_COSTS](#ARE-EDITABLE-ACTUAL-COSTS) | Determina se i costi effettivi sono modificabili. |
| [AUTHOR](#AUTHOR) | L'autore di un progetto. |
| [AUTOLINK](#AUTOLINK) | Determina se le attività inserite o spostate sono collegate automaticamente. |
| [AUTO_ADD_NEW_RESOURCES_AND_TASKS](#AUTO-ADD-NEW-RESOURCES-AND-TASKS) | Determina se nuove risorse o attività vengono aggiunte automaticamente a un pool di risorse o attività. |
| [AUTO_CALCULATE_ASSIGNMENT_COSTS](#AUTO-CALCULATE-ASSIGNMENT-COSTS) | Determina se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente utilizzando il lavoro dell'assegnazione e le tariffe delle risorse. |
| [BASELINE_FOR_EARNED_VALUE](#BASELINE-FOR-EARNED-VALUE) | La baseline specifica utilizzata per calcolare i valori di varianza. |
| [CALENDAR](#CALENDAR) | Il calendario del progetto. |
| [CATEGORY](#CATEGORY) | La categoria di un progetto. |
| [COMMENTS](#COMMENTS) | Commenti del progetto. |
| [COMPANY](#COMPANY) | L'azienda in cui è stato creato un progetto. |
| [CREATION_DATE](#CREATION-DATE) | La data e l'ora in cui è stato creato un progetto. |
| [CRITICAL_SLACK_LIMIT](#CRITICAL-SLACK-LIMIT) | Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni. |
| [CURRENCY_CODE](#CURRENCY-CODE) | Il codice a tre lettere della valuta come definito nella ISO 4217. |
| [CURRENCY_DIGITS](#CURRENCY-DIGITS) | Il numero di cifre dopo il simbolo decimale. |
| [CURRENCY_SYMBOL](#CURRENCY-SYMBOL) | Il simbolo della valuta utilizzato in un progetto. |
| [CURRENCY_SYMBOL_POSITION](#CURRENCY-SYMBOL-POSITION) | La posizione del simbolo della valuta. |
| [CURRENT_DATE](#CURRENT-DATE) | La data di sistema. |
| [CUSTOM_DATE_FORMAT](#CUSTOM-DATE-FORMAT) | Formato data personalizzato della visualizzazione del progetto. |
| [DATE_FORMAT](#DATE-FORMAT) | Formato data della visualizzazione del progetto. |
| [DAYS_PER_MONTH](#DAYS-PER-MONTH) | Il numero di giorni per mese. |
| [DEFAULT_FINISH_TIME](#DEFAULT-FINISH-TIME) | L'ora di fine predefinita delle nuove attività. |
| [DEFAULT_FIXED_COST_ACCRUAL](#DEFAULT-FIXED-COST-ACCRUAL) | Il tipo predefinito quando i costi fissi sono accumulati. |
| [DEFAULT_OVERTIME_RATE](#DEFAULT-OVERTIME-RATE) | Il tasso di straordinario predefinito per le nuove risorse. |
| [DEFAULT_STANDARD_RATE](#DEFAULT-STANDARD-RATE) | Il tasso standard predefinito per le nuove risorse. |
| [DEFAULT_START_TIME](#DEFAULT-START-TIME) | L'ora di inizio predefinita delle nuove attività. |
| [DEFAULT_TASK_EV_METHOD](#DEFAULT-TASK-EV-METHOD) | Il metodo di valore guadagnato predefinito per le attività. |
| [DEFAULT_TASK_TYPE](#DEFAULT-TASK-TYPE) | Il tipo predefinito di nuove attività. |
| [DURATION_FORMAT](#DURATION-FORMAT) | Il formato per esprimere la durata complessiva. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | Il metodo predefinito per calcolare il valore guadagnato. |
| [EXTENDED_CREATION_DATE](#EXTENDED-CREATION-DATE) | Data utilizzata per il calcolo e la reportistica. |
| [FINISH_DATE](#FINISH-DATE) | La data di fine di un progetto. |
| [FISCAL_YEAR_START](#FISCAL-YEAR-START) | Determina se viene utilizzata la numerazione dell'anno fiscale. |
| [FY_START_DATE](#FY-START-DATE) | Il mese in cui inizia l'anno fiscale. |
| [GUID](#GUID) | Il GUID del progetto. |
| [HONOR_CONSTRAINTS](#HONOR-CONSTRAINTS) | Determina se le attività rispettano le loro date di vincolo. |
| [HYPERLINK_BASE](#HYPERLINK-BASE) | Base dei collegamenti ipertestuali del progetto. |
| [INSERTED_PROJECTS_LIKE_SUMMARY](#INSERTED-PROJECTS-LIKE-SUMMARY) | Determina se le sottoattività vengono calcolate come attività riepilogo. |
| [KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED](#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED) | Determina se le attività manuali devono essere mantenute al più vicino orario lavorativo quando vengono impostate come programmate automaticamente. |
| [KEYWORDS](#KEYWORDS) | Parole chiave del progetto. |
| [LAST_AUTHOR](#LAST-AUTHOR) | Ultimo autore del progetto. |
| [LAST_PRINTED](#LAST-PRINTED) | Ultimo orario di stampa del progetto. |
| [LAST_SAVED](#LAST-SAVED) | La data in cui un progetto è stato salvato l'ultima volta. |
| [MANAGER](#MANAGER) | Il responsabile di un progetto. |
| [MICROSOFT_PROJECT_SERVER_URL](#MICROSOFT-PROJECT-SERVER-URL) | Determina se un progetto è stato creato da un utente di Project Server rispetto a un utente NT. |
| [MINUTES_PER_DAY](#MINUTES-PER-DAY) | Il numero di minuti al giorno. |
| [MINUTES_PER_WEEK](#MINUTES-PER-WEEK) | Il numero di minuti alla settimana. |
| [MOVE_COMPLETED_ENDS_BACK](#MOVE-COMPLETED-ENDS-BACK) | Determina se la fine delle parti completate delle attività programmate per iniziare dopo la data di stato ma avviate prima deve essere riportata indietro alla data di stato. |
| [MOVE_COMPLETED_ENDS_FORWARD](#MOVE-COMPLETED-ENDS-FORWARD) | Determina se la fine delle parti completate delle attività programmate per essere completate prima della data di stato ma iniziate più tardi deve essere spostata avanti alla data di stato. |
| [MOVE_REMAINING_STARTS_BACK](#MOVE-REMAINING-STARTS-BACK) | Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare dopo la data di stato ma avviate prima deve essere riportato indietro alla data di stato. |
| [MOVE_REMAINING_STARTS_FORWARD](#MOVE-REMAINING-STARTS-FORWARD) | Determina se l'inizio delle parti rimanenti delle attività programmate per essere avviate più tardi deve essere spostato avanti alla data di stato. |
| [MULTIPLE_CRITICAL_PATHS](#MULTIPLE-CRITICAL-PATHS) | Determina se vengono calcolati più percorsi critici. |
| [NAME](#NAME) | Il nome del progetto. |
| [NEW_TASKS_ARE_MANUAL](#NEW-TASKS-ARE-MANUAL) | Determina se le nuove attività vengono create come manuali. |
| [NEW_TASKS_EFFORT_DRIVEN](#NEW-TASKS-EFFORT-DRIVEN) | Determina se le nuove attività sono basate sullo sforzo. |
| [NEW_TASKS_ESTIMATED](#NEW-TASKS-ESTIMATED) | Determina se una durata stimata viene mostrata per impostazione predefinita. |
| [NEW_TASK_START_DATE](#NEW-TASK-START-DATE) | Il tipo di data di inizio predefinito per le nuove attività. |
| [PROJECT_EXTERNALLY_EDITED](#PROJECT-EXTERNALLY-EDITED) | Determina se il progetto è stato modificato esternamente. |
| [REMOVE_FILE_PROPERTIES](#REMOVE-FILE-PROPERTIES) | Determina se tutte le proprietà del file verranno rimosse al salvataggio. |
| [REVISION](#REVISION) | Il numero di volte in cui un progetto è stato salvato. |
| [SAVE_VERSION](#SAVE-VERSION) | La versione di Microsoft Office Project da cui è stato salvato un file di progetto. |
| [SCHEDULE_FROM_START](#SCHEDULE-FROM-START) | Determina se calcolare il programma del progetto in avanti dalla data di inizio. |
| [SHOW_PROJECT_SUMMARY_TASK](#SHOW-PROJECT-SUMMARY-TASK) | Determina se visualizzare le informazioni di riepilogo di un intero progetto in un'unica riga con la propria barra di attività di riepilogo nella parte superiore della visualizzazione del diagramma di Gantt. |
| [SPLITS_IN_PROGRESS_TASKS](#SPLITS-IN-PROGRESS-TASKS) | Determina se le attività in corso possono essere suddivise. |
| [SPREAD_ACTUAL_COST](#SPREAD-ACTUAL-COST) | Determina se i costi effettivi vengono distribuiti alla data di stato. |
| [SPREAD_PERCENT_COMPLETE](#SPREAD-PERCENT-COMPLETE) | Determina se la percentuale di completamento viene distribuita alla data di stato. |
| [START_DATE](#START-DATE) | La data di inizio di un progetto. |
| [STATUS_DATE](#STATUS-DATE) | la data di stato per visualizzare i progressi o per calcolare i totali del valore guadagnato. |
| [SUBJECT](#SUBJECT) | L'oggetto di un progetto. |
| [TASK_UPDATES_RESOURCE](#TASK-UPDATES-RESOURCE) | Determina se gli aggiornamenti alle attività aggiornano le risorse. |
| [TEMPLATE](#TEMPLATE) | Modello del progetto. |
| [TIMESCALE_FINISH](#TIMESCALE-FINISH) | La data in cui la scala temporale nella visualizzazione termina. |
| [TIMESCALE_START](#TIMESCALE-START) | La data in cui la scala temporale nella visualizzazione inizia. |
| [TITLE](#TITLE) | Il titolo di un progetto. |
| [UID](#UID) | L'ID univoco di un progetto. |
| [UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS](#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS) | Determina se le attività manuali devono essere aggiornate quando i collegamenti sono stati modificati. |
| [WEEK_START_DAY](#WEEK-START-DAY) | Primo giorno della settimana. |
| [WORK_FORMAT](#WORK-FORMAT) | Il formato usato per mostrare la durata dell'attività. |
### ACTUALS_IN_SYNC {#ACTUALS-IN-SYNC}
```
public static final Key<NullableBool,Byte> ACTUALS_IN_SYNC
```


Determina se tutti i lavori effettivi sono stati sincronizzati con il progetto.

### ADMIN_PROJECT {#ADMIN-PROJECT}
```
public static final Key<NullableBool,Byte> ADMIN_PROJECT
```


Determina se un progetto è un progetto amministrativo.

### ARE_EDITABLE_ACTUAL_COSTS {#ARE-EDITABLE-ACTUAL-COSTS}
```
public static final Key<NullableBool,Byte> ARE_EDITABLE_ACTUAL_COSTS
```


Determina se i costi effettivi sono modificabili.

### AUTHOR {#AUTHOR}
```
public static final Key<String,Byte> AUTHOR
```


L'autore di un progetto.

### AUTOLINK {#AUTOLINK}
```
public static final Key<NullableBool,Byte> AUTOLINK
```


Determina se le attività inserite o spostate sono collegate automaticamente.

### AUTO_ADD_NEW_RESOURCES_AND_TASKS {#AUTO-ADD-NEW-RESOURCES-AND-TASKS}
```
public static final Key<NullableBool,Byte> AUTO_ADD_NEW_RESOURCES_AND_TASKS
```


Determina se nuove risorse o attività vengono aggiunte automaticamente a un pool di risorse o attività.

### AUTO_CALCULATE_ASSIGNMENT_COSTS {#AUTO-CALCULATE-ASSIGNMENT-COSTS}
```
public static final Key<Boolean,Byte> AUTO_CALCULATE_ASSIGNMENT_COSTS
```


Determina se il costo dell'assegnazione e il costo residuo devono essere calcolati automaticamente utilizzando il lavoro dell'assegnazione e le tariffe delle risorse.

### BASELINE_FOR_EARNED_VALUE {#BASELINE-FOR-EARNED-VALUE}
```
public static final Key<Integer,Byte> BASELINE_FOR_EARNED_VALUE
```


La baseline specifica utilizzata per calcolare i valori di varianza.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


Il calendario del progetto.

### CATEGORY {#CATEGORY}
```
public static final Key<String,Byte> CATEGORY
```


La categoria di un progetto.

### COMMENTS {#COMMENTS}
```
public static final Key<String,Byte> COMMENTS
```


Commenti del progetto.

### COMPANY {#COMPANY}
```
public static final Key<String,Byte> COMPANY
```


L'azienda in cui è stato creato un progetto.

### CREATION_DATE {#CREATION-DATE}
```
public static final Key<Date,Byte> CREATION_DATE
```


La data e l'ora in cui è stato creato un progetto.

--------------------

Salvato in formato UTC nei file mpp. Tipo java.util.Date.

### CRITICAL_SLACK_LIMIT {#CRITICAL-SLACK-LIMIT}
```
public static final Key<Integer,Byte> CRITICAL_SLACK_LIMIT
```


Le attività sono considerate critiche da MS Project se il margine totale è inferiore o uguale a questo numero di giorni.

### CURRENCY_CODE {#CURRENCY-CODE}
```
public static final Key<String,Byte> CURRENCY_CODE
```


Il codice di valuta a tre lettere definito in ISO 4217. Un esempio di valori validi è "USD".

### CURRENCY_DIGITS {#CURRENCY-DIGITS}
```
public static final Key<Integer,Byte> CURRENCY_DIGITS
```


Il numero di cifre dopo il simbolo decimale.

### CURRENCY_SYMBOL {#CURRENCY-SYMBOL}
```
public static final Key<String,Byte> CURRENCY_SYMBOL
```


Il simbolo della valuta utilizzato in un progetto.

### CURRENCY_SYMBOL_POSITION {#CURRENCY-SYMBOL-POSITION}
```
public static final Key<Integer,Byte> CURRENCY_SYMBOL_POSITION
```


La posizione del simbolo della valuta.

### CURRENT_DATE {#CURRENT-DATE}
```
public static final Key<Date,Byte> CURRENT_DATE
```


La data di sistema.

### CUSTOM_DATE_FORMAT {#CUSTOM-DATE-FORMAT}
```
public static final Key<String,Byte> CUSTOM_DATE_FORMAT
```


Formato data personalizzato della vista progetto. Usato per formattare le date quando la proprietà [DATE\_FORMAT](../../com.aspose/tasks/prj\#DATE-FORMAT) è impostata su [DateFormat.Custom](../../com.aspose/tasks/dateformat\#Custom).

### DATE_FORMAT {#DATE-FORMAT}
```
public static final Key<Integer,Byte> DATE_FORMAT
```


Formato data della visualizzazione del progetto.

### DAYS_PER_MONTH {#DAYS-PER-MONTH}
```
public static final Key<Integer,Byte> DAYS_PER_MONTH
```


Il numero di giorni per mese.

### DEFAULT_FINISH_TIME {#DEFAULT-FINISH-TIME}
```
public static final Key<Date,Byte> DEFAULT_FINISH_TIME
```


L'ora di fine predefinita delle nuove attività.

### DEFAULT_FIXED_COST_ACCRUAL {#DEFAULT-FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> DEFAULT_FIXED_COST_ACCRUAL
```


Il tipo predefinito quando i costi fissi sono accumulati.

### DEFAULT_OVERTIME_RATE {#DEFAULT-OVERTIME-RATE}
```
public static final Key<Double,Byte> DEFAULT_OVERTIME_RATE
```


Il tasso di straordinario predefinito per le nuove risorse.

### DEFAULT_STANDARD_RATE {#DEFAULT-STANDARD-RATE}
```
public static final Key<Double,Byte> DEFAULT_STANDARD_RATE
```


Il tasso standard predefinito per le nuove risorse.

### DEFAULT_START_TIME {#DEFAULT-START-TIME}
```
public static final Key<Date,Byte> DEFAULT_START_TIME
```


L'ora di inizio predefinita delle nuove attività.

### DEFAULT_TASK_EV_METHOD {#DEFAULT-TASK-EV-METHOD}
```
public static final Key<Integer,Byte> DEFAULT_TASK_EV_METHOD
```


Il metodo di valore guadagnato predefinito per le attività.

### DEFAULT_TASK_TYPE {#DEFAULT-TASK-TYPE}
```
public static final Key<Integer,Byte> DEFAULT_TASK_TYPE
```


Il tipo predefinito di nuove attività.

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Byte,Byte> DURATION_FORMAT
```


Il formato per esprimere la durata complessiva. Tipo `TimeUnitType`.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


Il metodo predefinito per calcolare il valore guadagnato.

### EXTENDED_CREATION_DATE {#EXTENDED-CREATION-DATE}
```
public static final Key<Date,Byte> EXTENDED_CREATION_DATE
```


Data utilizzata per il calcolo e la reportistica.

### FINISH_DATE {#FINISH-DATE}
```
public static final Key<Date,Byte> FINISH_DATE
```


La data di fine di un progetto.

### FISCAL_YEAR_START {#FISCAL-YEAR-START}
```
public static final Key<NullableBool,Byte> FISCAL_YEAR_START
```


Determina se viene utilizzata la numerazione dell'anno fiscale.

### FY_START_DATE {#FY-START-DATE}
```
public static final Key<Integer,Byte> FY_START_DATE
```


Il mese in cui inizia l'anno fiscale.

### GUID {#GUID}
```
public static final Key<UUID,Byte> GUID
```


Il GUID del progetto.

### HONOR_CONSTRAINTS {#HONOR-CONSTRAINTS}
```
public static final Key<NullableBool,Byte> HONOR_CONSTRAINTS
```


Determina se le attività rispettano le loro date di vincolo.

### HYPERLINK_BASE {#HYPERLINK-BASE}
```
public static final Key<String,Byte> HYPERLINK_BASE
```


Base dei collegamenti ipertestuali del progetto.

### INSERTED_PROJECTS_LIKE_SUMMARY {#INSERTED-PROJECTS-LIKE-SUMMARY}
```
public static final Key<NullableBool,Byte> INSERTED_PROJECTS_LIKE_SUMMARY
```


Determina se le sottoattività vengono calcolate come attività riepilogo.

### KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED {#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED}
```
public static final Key<NullableBool,Byte> KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED
```


Determina se le attività manuali devono essere mantenute al più vicino orario lavorativo quando vengono impostate come programmate automaticamente.

### KEYWORDS {#KEYWORDS}
```
public static final Key<String,Byte> KEYWORDS
```


Parole chiave del progetto.

### LAST_AUTHOR {#LAST-AUTHOR}
```
public static final Key<String,Byte> LAST_AUTHOR
```


Ultimo autore del progetto.

### LAST_PRINTED {#LAST-PRINTED}
```
public static final Key<Date,Byte> LAST_PRINTED
```


Ultimo orario di stampa del progetto.

--------------------

Salvato in formato UTC nei file mpp. Tipo java.util.Date.

### LAST_SAVED {#LAST-SAVED}
```
public static final Key<Date,Byte> LAST_SAVED
```


La data in cui un progetto è stato salvato l'ultima volta.

--------------------

Salvato in formato UTC nei file mpp. Tipo java.util.Date.

### MANAGER {#MANAGER}
```
public static final Key<String,Byte> MANAGER
```


Il responsabile di un progetto.

### MICROSOFT_PROJECT_SERVER_URL {#MICROSOFT-PROJECT-SERVER-URL}
```
public static final Key<NullableBool,Byte> MICROSOFT_PROJECT_SERVER_URL
```


Determina se un progetto è stato creato da un utente di Project Server rispetto a un utente NT.

### MINUTES_PER_DAY {#MINUTES-PER-DAY}
```
public static final Key<Integer,Byte> MINUTES_PER_DAY
```


Il numero di minuti al giorno.

### MINUTES_PER_WEEK {#MINUTES-PER-WEEK}
```
public static final Key<Integer,Byte> MINUTES_PER_WEEK
```


Il numero di minuti alla settimana.

### MOVE_COMPLETED_ENDS_BACK {#MOVE-COMPLETED-ENDS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_BACK
```


Determina se la fine delle parti completate delle attività programmate per iniziare dopo la data di stato ma avviate prima deve essere riportata indietro alla data di stato.

### MOVE_COMPLETED_ENDS_FORWARD {#MOVE-COMPLETED-ENDS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_FORWARD
```


Determina se la fine delle parti completate delle attività programmate per essere completate prima della data di stato ma iniziate più tardi deve essere spostata avanti alla data di stato.

### MOVE_REMAINING_STARTS_BACK {#MOVE-REMAINING-STARTS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_BACK
```


Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare dopo la data di stato ma avviate prima deve essere riportato indietro alla data di stato.

### MOVE_REMAINING_STARTS_FORWARD {#MOVE-REMAINING-STARTS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_FORWARD
```


Determina se l'inizio delle parti rimanenti delle attività programmate per essere avviate più tardi deve essere spostato avanti alla data di stato.

### MULTIPLE_CRITICAL_PATHS {#MULTIPLE-CRITICAL-PATHS}
```
public static final Key<NullableBool,Byte> MULTIPLE_CRITICAL_PATHS
```


Determina se vengono calcolati più percorsi critici.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


Il nome del progetto.

### NEW_TASKS_ARE_MANUAL {#NEW-TASKS-ARE-MANUAL}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ARE_MANUAL
```


Determina se le nuove attività vengono create come manuali.

### NEW_TASKS_EFFORT_DRIVEN {#NEW-TASKS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> NEW_TASKS_EFFORT_DRIVEN
```


Determina se le nuove attività sono basate sullo sforzo.

### NEW_TASKS_ESTIMATED {#NEW-TASKS-ESTIMATED}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ESTIMATED
```


Determina se una durata stimata viene mostrata per impostazione predefinita.

### NEW_TASK_START_DATE {#NEW-TASK-START-DATE}
```
public static final Key<Integer,Byte> NEW_TASK_START_DATE
```


Il tipo di data di inizio predefinito per le nuove attività.

### PROJECT_EXTERNALLY_EDITED {#PROJECT-EXTERNALLY-EDITED}
```
public static final Key<NullableBool,Byte> PROJECT_EXTERNALLY_EDITED
```


Determina se il progetto è stato modificato esternamente.

### REMOVE_FILE_PROPERTIES {#REMOVE-FILE-PROPERTIES}
```
public static final Key<NullableBool,Byte> REMOVE_FILE_PROPERTIES
```


Determina se tutte le proprietà del file verranno rimosse al salvataggio.

### REVISION {#REVISION}
```
public static final Key<Integer,Byte> REVISION
```


Il numero di volte in cui un progetto è stato salvato.

### SAVE_VERSION {#SAVE-VERSION}
```
public static final Key<Integer,Byte> SAVE_VERSION
```


La versione di Microsoft Office Project da cui è stato salvato un file di progetto.

### SCHEDULE_FROM_START {#SCHEDULE-FROM-START}
```
public static final Key<NullableBool,Byte> SCHEDULE_FROM_START
```


Determina se calcolare il programma del progetto in avanti dalla data di inizio.

### SHOW_PROJECT_SUMMARY_TASK {#SHOW-PROJECT-SUMMARY-TASK}
```
public static final Key<Boolean,Byte> SHOW_PROJECT_SUMMARY_TASK
```


Determina se visualizzare le informazioni di riepilogo di un intero progetto in un'unica riga con la propria barra di attività di riepilogo nella parte superiore della visualizzazione del diagramma di Gantt.

### SPLITS_IN_PROGRESS_TASKS {#SPLITS-IN-PROGRESS-TASKS}
```
public static final Key<NullableBool,Byte> SPLITS_IN_PROGRESS_TASKS
```


Determina se le attività in corso possono essere suddivise.

### SPREAD_ACTUAL_COST {#SPREAD-ACTUAL-COST}
```
public static final Key<NullableBool,Byte> SPREAD_ACTUAL_COST
```


Determina se i costi effettivi vengono distribuiti alla data di stato.

### SPREAD_PERCENT_COMPLETE {#SPREAD-PERCENT-COMPLETE}
```
public static final Key<NullableBool,Byte> SPREAD_PERCENT_COMPLETE
```


Determina se la percentuale di completamento viene distribuita alla data di stato.

### START_DATE {#START-DATE}
```
public static final Key<Date,Byte> START_DATE
```


La data di inizio di un progetto.

### STATUS_DATE {#STATUS-DATE}
```
public static final Key<Date,Byte> STATUS_DATE
```


la data di stato per visualizzare l'avanzamento o calcolare i totali del valore guadagnato. La data di stato è la stessa della data corrente (data di oggi) a meno che non venga specificata una data di stato diversa.

### SUBJECT {#SUBJECT}
```
public static final Key<String,Byte> SUBJECT
```


L'oggetto di un progetto.

### TASK_UPDATES_RESOURCE {#TASK-UPDATES-RESOURCE}
```
public static final Key<NullableBool,Byte> TASK_UPDATES_RESOURCE
```


Determina se gli aggiornamenti alle attività aggiornano le risorse.

### TEMPLATE {#TEMPLATE}
```
public static final Key<String,Byte> TEMPLATE
```


Modello del progetto.

### TIMESCALE_FINISH {#TIMESCALE-FINISH}
```
public static final Key<Date,Byte> TIMESCALE_FINISH
```


La data in cui la scala temporale nella visualizzazione termina.

### TIMESCALE_START {#TIMESCALE-START}
```
public static final Key<Date,Byte> TIMESCALE_START
```


La data in cui la scala temporale nella visualizzazione inizia.

### TITLE {#TITLE}
```
public static final Key<String,Byte> TITLE
```


Il titolo di un progetto.

### UID {#UID}
```
public static final Key<String,Byte> UID
```


L'ID univoco di un progetto.

### UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS {#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS}
```
public static final Key<NullableBool,Byte> UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS
```


Determina se le attività manuali devono essere aggiornate quando i collegamenti sono stati modificati.

### WEEK_START_DAY {#WEEK-START-DAY}
```
public static final Key<Integer,Byte> WEEK_START_DAY
```


Primo giorno della settimana.

### WORK_FORMAT {#WORK-FORMAT}
```
public static final Key<Byte,Byte> WORK_FORMAT
```


Il formato usato per mostrare la durata dell'attività.

