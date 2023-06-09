<p align="center">
  <a href="https://www.asternox.it/">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/LOGO-TRASPARENTE.png" alt="Logo di Asternox" height=72>
  </a>
  
<h1 align="center"><i>Design System</i> per ARTISTA</h1>
<p align="center"><i>NOTA: la seguente documentazione è in fase di costruzione.</i></p>

## Indice

- [Introduzione](#introduzione)
- [Fondamenta del design system](#fondamenta-design)
- [Principi del design system](#principi-design)



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

Inoltre, è importante considerare la comfort zone degli occhi, altresì le *attention areas* in cui gli occhi dell'utente sono più propensi a concentrarsi durante l'esperienza VR. Queste aree di attenzione possono variare a seconda del contesto e dell'interazione desiderata, ma in generale includono il campo visivo frontale e le aree periferiche. Bisogna assicurarsi che le informazioni cruciali e gli elementi interattivi siano posizionati all'interno di queste aree, in modo che gli utenti possano facilmente individuarli senza dover spostare eccessivamente gli occhi o la testa. Questa pratica è importante per migliorare la leggibilità, l'usabilità e ridurrà l'affaticamento degli occhi durante l'interazione VR.

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

## Fondamenta del *design system*
### Griglia e Layout
Il nostro *design system* utilizza un sistema di griglia flessibile per garantire un layout coerente e ben strutturato nelle interfacce utente. In particolare, la nostra griglia è composta da <strong>12 colonne della distanza (<i>gutter</i>) di 16px l'una</strong> (la scelta di 12 colonne consente di avere una flessibilità sufficiente per adattare il layout alle diverse dimensioni dello schermo o esigenze).

Di seguito è riportata una sintesi visiva del layout:

<img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/layout/Layout.png" alt="Layout generale di ARTISTA">

L'interfaccia si divide in due parti fondamentali: la <strong>view principale</strong> e la <strong>sidebar</strong>. Nella 
<img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/layout/Layout-Padding.png" alt="Layout generale di ARTISTA, compreso di padding">
<img src="https://github.com/AsternoxCode/artista_design_system/blob/22712699cefd3604578dc6d972eab206761bf556/layout/Layout-Padding-Schede.png" alt="Layout generale di ARTISTA, padding e schede">

Ed hanno le seguenti caratteristiche:

#### View principale
  
```bash
W: 736px
H: 560px
Corner radius: 12px
Fill: Solid
rgba(255, 255, 255, 0.55)
Stroke: Solid
#FFFFFF
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
#222222
```
#### Schede
  
```bash
W: 219px
H: 239px
Corner radius: 6px
Fill: Solid
rgba(255, 255, 255, 0.5)
Stroke: Solid
#222222
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
