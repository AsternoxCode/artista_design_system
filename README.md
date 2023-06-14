<p align="center">
  <a href="https://www.asternox.it/">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/LOGO-TRASPARENTE.png" alt="Logo di Asternox" height=72>
  </a>
  
<h1 align="center"><i>Design System</i> per ARTISTA</h1>
<p align="center"><i>NOTA: la seguente documentazione è in fase di costruzione.</i></p>

## Indice

- [Introduzione](#introduzione)
- [Principi del design system](#principi-design)
- [Fondamenta del design system](#fondamenta-design)
- Controlli

## Introduzione
Questo documento è progettato per fornire una panoramica del <i>design system</i> progettato da Asternox per il progetto ARTISTA, un sistema modellatore di *virtual pottery* in modalità VR (*Virtual Reality*) intuitivo ed essenziale; il software è destinato all'utilizzo da parte di utenti sia novizi che esperti che vogliono esplorare il potenziale creativo della ceramica.
Il documento comprende linee guida, componenti e risorse essenziali per garantire coerenza, efficienza e qualità nel progesso di progettazione e sviluppo.

### Obiettivi del *Design System*
Il nostro design system ha lo scopo di raggiungere diversi obiettivi chiave che ci permettono di migliorare la coerenza visiva, accelerare lo sviluppo dei prodotti e fornire un'esperienza utente superiore. Nel dettaglio:

1. **Coerenza:** fornire un insieme coerente di principi di design, componenti e linee guida per garantire un aspetto e un comportamento uniformi in tutti i nostri prodotti.
2. **Efficienza:** semplificare il processo di progettazione e sviluppo fornendo componenti riutilizzabili che consentono di creare prodotti in modo più rapido ed efficiente.
3. **Qualità:** garantire la qualità delle nostre interfacce utente attraverso l'adozione di buone pratiche di design e l'attenzione ai dettagli, migliorando l'esperienza complessiva degli utenti.
4. **Scalabilità:** creare un sistema modulare e scalabile che possa adattarsi alle esigenze del software nel presente e nel futuro, consentendo un'evoluzione continua dell'ecosistema di design.

## Principi del <i>design system</i>

### Progettazione per sistemi VR: *campo visivo* e *comfort zone degli occhi*
Quando si progetta per il software VR, è fondamentale tenere conto del campo visivo (*field of view* o FOV) e della comfort zone degli occhi, al fine di garantire un'esperienza utente ottimale e confortevole. Il campo visivo rappresenta l'area visiva che l'utente può vedere attraverso gli occhiali VR e può variare a seconda del dispositivo utilizzato; per sfruttare al meglio il campo visivo, è consigliato posizionare gli elementi chiave, come testi e icone, all'interno della zona di visione centrale dell'utente, in modo che siano facilmente leggibili e comprensibili.

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/general-design/FOV.png" height=300 alt="Immagine che rappresenta la field of view"> 
    <p align="center"><i>FOV - Fonte: <a href="https://developer.oculus.com/resources/bp-vision/" target="_blank">Oculus</a></i></p>
</p>

Inoltre, è importante considerare la comfort zone degli occhi, altresì le *attention areas* in cui gli occhi dell'utente sono più propensi a concentrarsi durante l'esperienza VR. Queste aree di attenzione possono variare a seconda del contesto e dell'interazione desiderata, ma in generale includono il campo visivo frontale e le aree periferiche. Bisogna assicurarsi che le informazioni cruciali e gli elementi interattivi siano posizionati all'interno di queste aree, in modo che gli utenti possano facilmente individuarli senza dover spostare eccessivamente gli occhi o la testa. Questa pratica è importante per migliorare la leggibilità, l'usabilità e ridurrà l'affaticamento degli occhi durante l'interazione VR.

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/general-design/AngularGrid.png" height=300 alt="Immagine che rappresenta la griglia angolare del campo visivo."> 
    <p align="center"><i>Griglia angolare del campo visivo</i></p>
</p>
  
<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/general-design/Attention%20Areas.png" height=300 alt="Immagine che rappresenta la griglia angolare del campo visivo in relazione alla comfort zone dell'occhio"> 
    <p align="center"><i>Griglia angolare del campo visivo con rappresentazione della comfort zone dell'occhio (e area di attenzione)</i></p>
</p>

Bisogna, infine, considerare anche altri aspetti tecnici, come il bilanciamento dei colori, il contrasto, la dimensione del testo e l'uso delle animazioni, al fine di garantire una buona leggibilità, una chiara comunicazione visiva e una navigazione intuitiva nell'ambiente VR.

### Principi fondamentali della progettazione UI per VR
- **Non utilizzare né il bianco puro né il nero puro.** Ciò vale per qualsiasi tipo di design dell'interfaccia utente, ma in VR provoca un disagio estremamente fastidioso, in quanto influisce sull'illuminazione globale. Posizionare il bianco puro è come esporsi alla luce quando gli occhi sono ancora in modalità notturna. Il nero e il bianco utilizzati per le interfacce di questo *design system* non sono **mai** puri; se lo sono, è legato soltanto al testo edè dovuto dalla necessità di dover fornire abbastanza contrasto all'utente.
- **Utilizzare caratteri con ampi spazi bianchi, evitare i caratteri stretti.** Quasi tutti i caratteri tipografici utilizzati di solito nelle UI saranno ottimali in VR, ma a causa delle risoluzioni inferiori (rispetto a quelle dei telefoni o di uno schermo) gli spazi non sono definiti al meglio; è fondamentale dare spazio ai pixel.
- **I colori tendono a essere più brillanti in VR.** Il contrasto tra i colori aumenta in VR, soprattutto quando si utilizzano applicazioni autonome. Gli oculus VR non hanno ancora la risoluzione che ci si aspetta da uno smartphone o da uno schermo retina, quindi la definizione e il contrasto non sono precisi come nei dispositivi tradizionali.
- **Comprendere distanze, altezze e aree di comfort.** Questo punto è fondamentale da considerare se il prodotto finale vuole essere in linea con il design iniziale: una distanza di 2 metri è molto diversa da quella di 1 metro. Anche la scala è la stessa: 1 metro dà una sensazione di vicinanza e di importanza, mentre 2 o 3 metri danno una sensazione di distanza e di tranquillità. Attenzione a non forzare mai il contenuto ma ad adattarlo.

### Principi guida
I seguenti principi di design sono la base di questo *design system*, e guidano l'approccio alla progettazione, aiutando nella creazione di esperienze coerenti, intuitive e coinvolgenti per gli utenti.

1. **Semplicità:** l'obiettivo è mantenere un approccio semplice e pulito nel design dell'interfaccia, riducendo l'elemento di confusione e concentrandosi su un'esperienza utente chiara ed efficace.
2. **Accessibilità:** l'obiettivo è favorire un design inclusivo che sia accessibile a tutti gli utenti, indipendentemente dalle loro capacità. Il design è stato progettato considerando le linee guida WCAG e buone pratiche per garantire un'esperienza fruibile per tutti.
3. **Coerenza:** l'obiettivo è promuovere la coerenza nell'aspetto e nel comportamento dell'interfaccia. Per tale motivo si è progettato un set di componenti condivisi e linee guida di design per garantire una sensazione uniforme in tutto l'ecosistema del prodotto.
4. **Flessibilità:** l'obiettivo è offrire una flessibilità adeguata a futuri design e sviluppatori per adattarsi a diverse situazioni e requisiti. I componenti sono progettati per essere personalizzabili e adattabili per soddisfare le esigenze specifiche del prodotto.
5. **Efficienza:** l'obiettivo è migliorare l'efficienza del lavoro fornendo un set di componenti e risorse riutilizzabili, riducendo il tempo necessario per progettare e sviluppare nuove interfacce, utilizzando i nostri principi di design come guida.

### *Information Architecture*
L'*information architecture* (abbr. IA) è la pratica dello UX Design volta ad organizzare, strutturare e progettare l'accesso alle informazioni in modo intuitivo ed efficiente. L'obiettivo dell'information architecture è quello di creare una struttura coerente e comprensibile per un sistema informativo.
L'IA si basa sulla comprensione delle esigenze degli utenti e dei contenuti informativi da presentare. Essendo l'IA correlata all'*interaction design*, all'usabilità e alla UX, essendo il nostro sistema *user-centered*, è importante creare un'architettura ottimizzata.

Creare un'IA efficace richiede un processo di progettazione o un approccio strutturato; creare una IA per un software VR richiede un approccio leggermente diverso rispetto a un'applicazione web o mobile. Nel dettaglio, è necessario considerare:

- **La comprensione piena dell'esperienza utente**, in particolare gli aspetti unici della VR, come la profondità, l'immersione e le interazioni spaziali, gli spostamenti nello spazio virtuale e il relazionamento con oggetti e contenuti;
- **La definizione di obiettivi e casi d'uso** come esplorazione di ambienti virtuali, l'interazione con oggetti o la visualizzazione di contenuti multimediali;
- **La progettazione della struttura spaziale**, che non è più bidimensionale. Bisogna considerare, infatti, profondità, altezza e posizione degli oggetti per creare una struttura spaziale intuitiva;
- **La progettazione di un'interfaccia intuitiva** (non solo della struttura spaziale), che sfrutti le capacità interattive della VR come tracciamento dei movimenti delle mani o dei controller, con feedback visivi e sonori;
- **La semantica degli oggetti e degli ambienti**, a cui si aggiunge una dimensione in più da sfruttare (non solo altezza e larghezza, ma anche profondità).

Essendo un menù "standard", il menù principale ha uno schema più semplice rispetto all'interfaccia di gioco. Ciò è dovuto anche all'approccio dell'applicazione più "tecnico" rispetto ad un gioco VR vero e proprio.

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/f0e20bd58e9c7b07bd45ba359291255a4e5b1892/general-design/Information-Architecture-Main.png" height=500 alt="Information Architecture del menù principale"> 
    <p align="center"><i>Information Architecture del menù principale</i></p>
</p>

## Fondamenta del *design system*

### Griglia e Layout
Il nostro *design system* utilizza un sistema di griglia flessibile per garantire un layout coerente e ben strutturato nelle interfacce utente. In particolare, la griglia è composta da <strong>12 colonne della distanza (<i>gutter</i>) di 16px l'una</strong> (la scelta di 12 colonne consente di avere una flessibilità sufficiente per adattare il layout alle diverse dimensioni dello schermo o esigenze).

Di seguito è riportata una sintesi visiva della griglia layout. La stessa sintesi visiva è riportata in relazione alla FOV e all'area di attenzione: è evidente dall'immagine come il layout scelto si adatti naturalmente alla comfort zone dell'occhio e come gli elementi principali della schermata siano i primi ad essere recepiti dall'utente.

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/layout/Layout.png" height=500 alt="Layout del sistema."> 
    <p align="center"><i>Layout generale del sistema.</i></p>
</p>

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/general-design/Griglie-AngularGrid.png" height=300 alt="Layout dell'interfaccia in relazione al FOV."> 
    <p align="center"><i>Layout in relazione al FOV.</i></p>
</p>

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/general-design/Griglie-AttentionAreas.png" height=300 alt="Layout dell'interfaccia in relazione alle attention area."> 
    <p align="center"><i>Layout in relazione alle attention area.</i></p>
</p>

### *View* principale e *sidebar*

L'interfaccia si divide in due parti fondamentali: la <strong>view principale</strong> e la <strong>sidebar</strong>.
La *view* principale è caratterizzata dagli elementi di interazione principali, mentre la sidebar fornisce navigazione; solo occasionalmente quest'ultima è l'elemento principale, in particolare quando l'interazione utente con l'interfaccia è di passaggio (quasi immediata e caratterizzata da poche interazioni).

Il layout delle interfacce è predisposto come segue:

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/layout/Layout-Padding.png" height=500 alt="Layout della view principale e della sidebar, in particolare il cd. padding."> 
    <p align="center"><i>Layout della view principale e della sidebar, in particolare il cd. padding.</p>
</p>

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/7b60245d184b64c3fcd64a7c6c7c8176cf5920ed/layout/Layout-Padding-Schede.png" height=500 alt="Layout della view principale e della sidebar, in particolare il cd. padding."> 
    <p align="center"><i>Layout della view principale e della sidebar, in particolare il cd. padding, con l'aggiunta di più elementi (come le schede).</p>
</p>


#### View principale
  
```bash
W: 736px
H: 560px
Corner radius: 12px
Fill: Solid
rgba(255, 255, 255, 0.55)
Stroke: Solid
hex FFFFFF
Align: Center
Width: 2px
Effect: Background blur
Radius: 10px
```

#### Sidebar

```bash
W: 256px
H: 560px
Corner radius: 12px
Fill: Solid
hex 222222
```
#### Schede
  
```bash
W: 219px
H: 239px
Corner radius: 6px
Fill: Solid
rgba(255, 255, 255, 0.5)
Stroke: Solid
hex 222222
Align: Inside
Width: 1px
```

### Tipografia

Il font utilizzato è [Poppins](https://fonts.google.com/specimen/Poppins).

Poppins è un font moderno e pulito caratterizzato da forme arrotondate che lo rendono accessibile e amichevole. La sua ampia gamma di stili e pesi consente una maggiore flessibilità nell'adattamento del testo a diverse dimensioni e dispositivi. È progettato con una buona leggibilità, con una distinzione chiara tra le lettere simili, migliorando l'esperienza di lettura per gli utenti. La sua eleganza e precisione conferiscono al font un aspetto professionale e raffinato, adatto a progetti che richiedono un tocco di sofisticatezza. Nel complesso, Poppins unisce accessibilità, professionalità e leggibilità, rendendolo una scelta solida per l'interfaccia del tuo software di modellazione 3D per artigiani digitali.

|   Tipo           | Ag | Weight | Size | Line height | Letter |
|------------------|----|--------|------|-------------|--------|
| Header 1         | H1 |  700   | 32px |  38px       | 1px    |
| Header 2         | H2 |  700   | 26px |  32px       | 1px    |
| Header 3         | H3 |  700   | 20px |  27px       | 0.5px  |
| Header 4         | H4 |  700   | 16px |  27px       | 0.5px  |
|  Titolo          | T0 |  500   | 16px |  24px       | 1px    |
|  Corpo           | C1 |  500   | 16px |  24px       | 0.5px  |
|  Corpo 2         | C2 |  500   | 14px |  21px       | 0.5px  |
|  Corpo 3         | C3 |  500   | 12px |  18px       | 1px    |
| Pulsante grande  | PG |  500   | 18px |  28px       | 1px    |
| Pulsante medio   | PM |  500   | 16px |  26px       | 0.5px  |
| Pulsante piccolo | PP |  500   | 14px |  26px       | 0.5px  |

### Sistema di colori
Il design system di ARTISTA offre un sistema di colori ben definito che consente di mantenere una coerenza visiva in tutto il software, soprattutto coinvolgente e confortevole, essendo destinata ad un ambiente VR. La scelta dei colori è cruciale per guidare l'attenzione dell'utente, comunicare informazioni importanti e creare un'atmosfera coerente all'interno dell'ambiente VR.

#### Utilizzo dei colori in un'interfaccia VR

In una interfaccia VR è importante utilizzare i colori in modo strategico per guidare l'utente e creare un'esperienza visiva armoniosa. Alcune considerazioni effettuate nella creazione del sistema di colori:

- **Contrasto:** è essenziale assicurarsi che vi sia un contrasto sufficiente tra i colori degli elementi interattivi e lo sfondo circostante ;questo migliorerà la leggibilità e facilita l'individuazione degli elementi interattivi nell'ambiente VR.
- **Feedback visivo:** è consigliato utilizzare i colori per fornire feedback visivi all'utente, come ad esempio una variazione di colore per indicare quando un'azione è stata completata con successo o per evidenziare un elemento selezionato.
- **Scala cromatica:** utilizzare tonalità e sfumature della stessa famiglia di colori per creare una scala cromatica coerente all'interno dell'interfaccia VR. Questo contribuirà a creare una sensazione di coesione visiva e fluidità all'interno dell'ambiente virtuale.
- **Considerazioni per la visione stereoscopica:** tenendo conto della natura stereoscopica dell'ambiente VR, evitare l'utilizzo di colori che possono causare distorsioni visive o effetti indesiderati nell'esperienza stereoscopica dell'utente.

#### Sintesi visiva del sistema di colori

L'immagine di seguito riporta una sintesi visiva del sistema di colori. La tabella, invece, riporta i codici degli stessi.

<p align="center">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/f0e20bd58e9c7b07bd45ba359291255a4e5b1892/general-design/COLORI.png" height=1000 alt="Sistema di colori di ARTISTA"> 
    <p align="center"><i>Sistema di colori di ARTISTA</i></p>
</p>

|     Colori neutri    |    Primary, Azioni    | Primary, Sfumature | Primary, Azioni sfumature |   Primary, Stati   |         Testo         |
|----------------------|-----------------------|--------------------|---------------------------|--------------------|-----------------------|
| Interfaccia - 222222 | Default - 595959      | 900 - 410A0C       | Principale - C21D24       | Hover - A2181E     | Primary - FFFFFF      |
| Grigio 2 - 2B2B2B    | Hover - 525252        | 800 - 610E12       | Dark - A2181E             | Default - C21D24   | Secondary - EEEEEE    |
| Grigio 3 - 363636    | Attivo - 686868       | 700 - 811318       | Light - E64442            | Attivo - E64442    | Disabilitato - 818181 |
| Grigio 4 - 404040    | Disabilitato - 595959 | 600 - A2181E       | Link - EA6361             | Contrasto - FF6C6C |                       |
| Grigio 5 - 595959    |                       | 500 - C21D24       |                           |                    |                       |
| Grigio 6 - 686868    |                       | 400 - CC4349       |                           |                    |                       |
| Grigio 7 - 909090    |                       | 300 - D6686D       |                           |                    |                       |
| Grigio 8 - B5B5B5    |                       | 200 - E08E92       |                           |                    |                       |
| Grigio 9 - D3D3D3    |                       | 100 - EBB4B6       |                           |                    |                       |
| Grigio 10 - EEEEEE   |                       | 050 - F3D2D3       |                           |                    |                       |
| Bianco - FFFFFF      |                       |                    |                           |                    |                       |

### Icone
Le icone rivestono un ruolo fondamentale nella comunicazione visiva all'interno di un software VR. Il design system di ARTISTA offre una vasta gamma di icone adatte specificamente per l'ambiente VR, consentendo una comunicazione rapida ed efficace delle informazioni agli utenti. La libreria di icone è completa e accessibile, e contiene una varietà di simboli e rappresentazioni visive ottimizzate per garantire la chiarezza e la leggibilità all'interno dell'ambiente virtuale.
Le icone sono disponibili in stile pieno e arrotondato, adatto alla coerenza visiva di tutta l'interfaccia. I formati dei file sono in PNG e SVG, adatti a Unity (da inserire in una cartella a parte).

Si raccomanda di utilizzare le icone del design system in modo coerente all'interno del tuo progetto per garantire un'esperienza VR fluida e una chiarezza visiva.

#### Personalizzazione
Nel contesto dell'ambiente VR in Unity, è possibile personalizzare le icone per adattarle ai tuoi specifici contesti o esigenze di progettazione; è possibile regolare la dimensione, il colore o l'animazione delle icone per integrarle perfettamente nell' ambiente VR. Tuttavia, è importante mantenere una coerenza visiva all'interno del sistema e utilizzare le personalizzazioni con attenzione per evitare sovraccarichi visivi o confusione per l'utente. Si consiglia, genericamente, di mantenere le animazioni e le transizioni il più semplici possibile.

## Componenti
Il design system di ARTISTA offre un set di componenti predefiniti. Questi componenti semplificano il processo di progettazione e sviluppo, garantendo coerenza vsiva e funzionale nelle schermate di ARTISTA.

### Bottoni
I bottoni (o pulsanti) sono elementi essenziali per l'interazione degli utenti con il software. Il design system di ARTISTA offre una varietà di stili e dimensioni di bottoni diversi, che possono essere utilizzati in base alle esigenze del progetto.
Abbiamo definito diversi stili di bottoni per adattarsi alle diverse azioni e al contesto di utilizzo.
Vi sono tre grandezze di default:

- GRANDE (G) 
height: 52px |
width: 186px |
border-radius: 10px |
padding: 12px 24px 12px 24px;

- MEDIO (M)
height: 42px |
width: 157px |
border-radius: 6px |
padding: 8px 16px 8px 16px;

- PICCOLO (P)
height: 32px |
width: 128px |
border-radius: 6px |
padding: 3px 14px 3px 14px;

Ogni bottone, quindi ogni grandezza, ha uno stile predefinito:

- **Primary:** bottoni utilizzati per le azioni principali dell'interfaccia. Questo stile di bottone è caratterizzato da un colore distintivo che richiama l'attenzione dell'utente.
- **Secondary:** bottoni utilizzati per le azioni secondarie o opzionali. Questi bottoni hanno un aspetto più sobrio.
- **Tertiary:** bottoni utilizzati per fornire un'interazione testuale o come collegamento senza l'aspetto tradizionale di un bottone. Generalmente utilizzato per azioni di minor rilevanza o per fornire informazioni aggiuntive.

Ogni stile predefinito, inoltre, è caratterizzato da:
- **Icona:** assenza o presenza dell'icona, che può essere a destra o a sinistra;
- **Stato del bottone:** ovvero interazione effettuata o possibile con il bottone, che si dividono in DEFAULT, HOVER, PREMUTO E DISABILITATO.

Ricapitolando, ogni bottone è determinato da:
- **DIMENSIONE:** GRANDE | MEDIO | PICCOLO;
- **TIPO:** PRIMARY | SECONDARY | TERTIARY;
- **ICONA:** NO | DX | SX;
- **STATO:** DEFAULT | HOVER | PREMUTO | DISABILITATO.

#### Impostazioni dei bottoni in Unity
In Unity vi sono delle impostazioni principali associate ad ogni tipologia di bottone, di seguito riassunte:

- **Target Graphic:** impostazione per definire l'immagine o il componente grafico che rappresenta il bottone. Questo componente determina l'aspetto visivo del bottone. Nel caso di questo design system è sufficiente creare un elemento grafico dedicato.
- **Transition:** impostazione per definire come il bottone reagisce quando viene interagito dall'utente.
- **Normal Color:** impostazione per definire il colore predefinito del bottone quando non è stato selezionato o interagito.
- **Highlighted Color:** impostazione per definire il colore che viene visualizzato quando il cursore del mouse è sopra il bottone (ovvero, corrisponde al feedback visivo dell'hovering).
- **Pressed Color:** impostazione per definire il colore che viene visualizzato quando il bottone viene premuto o selezionato. Buona norma è rendere il colore più scuro o più evidente per indicare che il bottone è stato attivato.
- **Disabled Color:** impostrazione per definire il colore che viene visualizzato quando il bottone è disabilitato, ovvero quando non può essere selezionato o interagito. Indicare che il bottone non è attualmente disponibile.

In base a queste impostazioni, possiamo definire una palette di colori per ogni stato e per ogni tipo di bottone (*primary*, *secondary* e *tertiary*):

##### Primary
- TESTO: FFFFFF, rgb(255, 255, 255, 100);
- TRANSITION: COLOR TINT
- NORMAL COLOR: C21D24, rgb(194, 29, 36, 100);
- HIGHLITED COLOR: A2181E, rgb(162, 24, 30, 100);
- PRESSED COLOR: E64442, rgb(230, 68, 66, 100);
- DISABLED COLOR: 595959, rgb(89, 89, 89, 100); E TESTO 818181, rgb(129, 129, 129, 100);

##### Tertiary
- TESTO: FFFFFF, rgb(255, 255, 255, 100);
- TRANSITION: COLOR TINT
- NORMAL COLOR: 595959, rgb(89, 89, 89, 100);
- HIGHLITED COLOR: 525252, rgb(82, 82, 82, 100);
- PRESSED COLOR: 686868, rgb(104, 104, 104, 100);
- DISABLED COLOR: 595959, rgb(89, 89, 89, 100); E TESTO 818181, rgb(129, 129, 129, 100);

I bottoni **Secondary** sono leggermente diversi, poiché presentano un contorno (*stroke*) e un'opacità.
Un metodo di sviluppo di un bottone del genere in Unity è il seguente:
1. **Creazione del bottone** tramite *UI > Button* nell'interfaccia di Unity;
2. **Creazione del contorno** creando un'immagine di sfondo per il bottone e impostando la sua dimensione in modo che sia leggermente più grande del bottone stesso;
3. **Gestione dell'opacità** regolando il valore dell'alpha del colore del bottone stesso o dell'immagine di sfondo sia tramite codice che attraverso l'editor di Unity.

#### Secondary
- TESTO: FFFFFF, rgb(255, 255, 255, 100);
- TRANSITION: COLOR TINT
- STROKE: C21D24, rgb(194, 29, 36, 1);
- NORMAL COLOR: C21D24 con 0% di alpha, rgb(194, 29, 36, 0);
- HIGHLITED COLOR: C21D24 con 20% di alpha, rgb(194, 29, 36, 0.2);
- PRESSED COLOR: C21D24 con 50% di alpha, rgb(194, 29, 36, 0.5);
- DISABLED COLOR: 595959, rgb(89, 89, 89, 100); E TESTO 818181, rgb(129, 129, 129, 100);

### Bottoni della sidebar
La *sidebar* presenta bottoni leggermente diversi, in particolare per la forma.
*in fase di scrittura*

## Controlli VR
*sezione in fase di scrittura*


