# signup
progetto asp.net
progettare un sito web con asp.net in cui, nella prima parte:

Il sito deve esporre nella barra di navigazione le pagine: Home, Privacy, SignUp, Purchase, Cart;
La pagina di SignUp deve contenere un form di registrazione;
Una volta compilato il form di SignUp l'utente deve essere rimandato ad una pagina di Riepilogo dei dati inseriti (tramite httpPost);
La pagina di Purchase deve esporre un form in cui l'utente possa inserire: nome del prodotto da acquistare, quantità di interesse;
Una volta compilato il form di Purchase l'utente deve essere rimandato alla pagina Cart, in cui comparirà l'elenco dei prodotti inseriti;
Modificare il progetto Signup&Purchase precedente in modo che utilizzi le variabili di sessione per fare login.
nella seconda parte il sito:

scriva sulla home page il nome dell'autore (o degli autori se siete in due) del progetto
preveda l'utilizzo di una form Login che preveda una backdoor (utente q e password q) utilizzando una variabile di sessione oppure un qualsiasi altro modo.
preveda di aggiungere un prodotto al carrello
preveda un link che visualizzi il carrello direttamente (dal menu) (solo se si è fatto login)
preveda una piccola icona a forma di cestino, in fondo ad ogni riga, che consenta di eliminare la riga
STRUTTURA DI UN PROGETTO ASP.NET la struttura di un progetto asp.net è definita da una serie di cartelle con diverse funzioni, quelle principali e su cui andremo a lavorare sono: -Controllers/: Questa cartella contiene i controller della tua applicazione che gestiranno le richieste HTTP e determinano quale logica di business o quale vista deve essere eseguita. All'interno di questa cartella si trova il file come HomeController.cs.

-Models/: Qui vengono definiti i modelli della tua applicazione. I modelli rappresentano i dati con cui l'applicazione lavora e definiscono la struttura dei dati (oggetti, classi) che possono essere utilizzati dai controller e dalle viste.

-Views/: Questa cartella contiene le viste dell'pplicazione. Le viste sono responsabili della presentazione dei dati agli utenti. La cartella è strutturata in base ai controller, nel nostro caso l'HomeController. All'interno di queste sottocartelle troviamo i file .cshtml che rappresentano le viste (ad esempio Index.cshtml).

-Views/Shared/: Questa sottocartella contiene le viste condivise tra più controller, quindi _Layout.cshtml definisce il layout principale dell'applicazione che può essere utilizzato da diverse viste e modificato per adattare la navbar alle esigenze dell'applicazione.

-wwwroot/: Questa cartella contiene i contenuti statici accessibili al client, come fogli di stile CSS, file JavaScript e librerie di terze parti come Bootstrap o jQuery. wwwroot/css/: Contiene i fogli di stile CSS dell'applicazione. wwwroot/js/: Contiene i file JavaScript dell'applicazione. wwwroot/lib/: Contiene le librerie di terze parti utilizzate nell'applicazione. è qui che i contenuti statici come le immagini andranno insserite per permetterne la visualizzazione nell'applicazione.

-Program.cs: Questo file rappresenta il punto di ingresso dell'applicazione. Contiene il metodo Main() che avvia l'applicazione.

-nome.Progetto.csproj: Questo è il file di progetto principale che definisce le dipendenze del progetto e altre impostazioni di compilazione. Qui anche quelle date dall'installazione dei pacchetti per il funzionamento di Entity Framework ed Sqlite.

Razor: Razor è un motore di visualizzazione che consente di integrare codice C# con HTML e altri elementi di markup all'interno di file CSHTML (C# HTML), permette di incorporare codice C# all'interno di un file CSHTML utilizzando la sintassi @{ ... }. Le direttive Razor, come @model, @using, consentono di definire il modello, di importare namespace e di ereditare da una classe base direttamente all'interno del file CSHTML. Altro grande vantaggio è quello di poter usare strutture (come i cicli) del c# direttamente nel file cshtml.

PAGINE BARRA DI NAVIGAZIONE:
