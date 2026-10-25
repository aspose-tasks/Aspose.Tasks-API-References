---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive quando il progetto viene salvato su Project Server o Project Online."
type: docs
weight: 227
url: /it/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Consente di specificare opzioni aggiuntive quando il progetto viene salvato su Project Server o Project Online.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Inizializza una nuova istanza della classe [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Ottiene l'intervallo tra le richieste di stato del lavoro in coda. |
| [getProjectGuid()](#getProjectGuid--) | Ottiene l'identificatore univoco di un progetto. |
| [getProjectName()](#getProjectName--) | Ottiene il nome di un progetto visualizzato nell'elenco dei progetti di Project Server \\\\ Project Online. |
| [getTimeout()](#getTimeout--) | Ottiene il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Imposta l'intervallo tra le richieste di stato del lavoro in coda. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Imposta l'identificatore univoco di un progetto. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Imposta il nome di un progetto visualizzato nell'elenco dei progetti di Project Server \\\\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | Imposta il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Inizializza una nuova istanza della classe [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Ottiene l'intervallo tra le richieste di stato del lavoro in coda. Il valore predefinito è 2 secondi.

**Returns:**
double - intervallo tra le richieste di stato del lavoro in coda.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Ottiene l'identificatore univoco di un progetto. Deve essere univoco all'interno dell'istanza di Project Server \\\\ Project Online.

**Returns:**
java.util.UUID - identificatore univoco di un progetto.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Ottiene il nome di un progetto visualizzato nell'elenco dei progetti di Project Server \\\\ Project Online. Deve essere univoco all'interno dell'istanza di Project Server \\\\ Project Online. Se il valore è omesso, verrà utilizzato il valore della proprietà Prj.Name.

**Returns:**
java.lang.String - nome di un progetto visualizzato nell'elenco dei progetti di Project Server \\\\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Ottiene il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. Il valore predefinito per questa proprietà è 1 minuto.

--------------------

Il tempo di elaborazione può essere più lungo per progetti di grandi dimensioni o nel caso in cui l'istanza di Project Server sia troppo occupata a rispondere ad altre richieste.

**Returns:**
double - timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Imposta l'intervallo tra le richieste di stato dei lavori in coda. Il valore predefinito è 2 secondi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | intervallo tra le richieste di stato dei lavori in coda. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Imposta l'identificatore univoco di un progetto. Deve essere unico all'interno dell'istanza di Project Server \ Project Online.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID | identificatore univoco di un progetto. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Imposta il nome di un progetto che viene visualizzato nell'elenco dei progetti di Project Server \ Project Online. Deve essere unico all'interno dell'istanza di Project Server \ Project Online. Se il valore viene omesso, verrà utilizzato il valore della proprietà Prj.Name.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | nome di un progetto che viene visualizzato nell'elenco dei progetti di Project Server \ Project Online. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Imposta il timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. Il valore predefinito per questa proprietà è 1 minuto.

--------------------

Il tempo di elaborazione può essere più lungo per progetti di grandi dimensioni o nel caso in cui l'istanza di Project Server sia troppo occupata a rispondere ad altre richieste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | timeout utilizzato durante l'attesa dell'elaborazione della richiesta di salvataggio del progetto da parte del servizio di elaborazione della coda di Project Server. |

