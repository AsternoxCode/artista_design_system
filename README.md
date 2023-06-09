<p align="center">
  <a href="https://www.asternox.it/">
    <img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/LOGO-TRASPARENTE.png" alt="Asternox Logo" height=72>
  </a>
  
<h1 align="center"><i>Design System</i> per ARTISTA</h3>

## Indice

- [Introduzione](#introduzione)
- [Principi del design system](#principi-design)
- [Fondamenta del design](#fondamenta-design)



## Introduzione
Questo documento è progettato per fornire una panoramica del <i>design system</i> progettato da Asternox per il progetto ARTISTA, un sistema modellatore di <i>virtual pottery</i> in modalità VR (<i>virtual reality </i>) intuitivo ed essenziale; il software è destinato all'utilizzo da parte di utenti sia novizi che esperti che vogliono esplorare il potenziale creativo della ceramica.
Il documento comprende linee guida, componenti e risorse essenziali per garantire coerenza, efficienza e qualità nel progesso di progettazione e sviluppo.

<h3>Obiettivi del <i>Design System</i></h3>
Il nostro design system ha lo scopo di raggiungere diversi obiettivi chiave che ci permettono di migliorare la coerenza visiva, accelerare lo sviluppo dei prodotti e fornire un'esperienza utente superiore. Nel dettaglio:

<ol>
  <li><b>Coerenza:</b> fornire un insieme coerente di principi di design, componenti e linee guida per garantire un aspetto e un comportamento uniformi in tutti i nostri prodotti.</li>
  <li><b>Efficienza:</b> semplificare il processo di progettazione e sviluppo fornendo componenti riutilizzabili che consentono di creare prodotti in modo più rapido ed efficiente.</li>
  <li><b>Qualità:</b> garantire la qualità delle nostre interfacce utente attraverso l'adozione di buone pratiche di design e l'attenzione ai dettagli, migliorando l'esperienza complessiva degli utenti.</li>
  <li><b>Scalabilità:</b> creare un sistema modulare e scalabile che possa adattarsi alle esigenze del software nel presente e nel futuro, consentendo un'evoluzione continua dell'ecosistema di design.</li>
</ol>

## Principi del <i>design system</i>
(sezione in fase di scrittura)


## Fondamenta del <i>design system</i>
<h3>Griglia e Layout</h3>
Il nostro design system utilizza un sistema di griglia flessibile per garantire un layout coerente e ben strutturato nelle interfacce utente. In particolare, la nostra griglia è composta da <strong>12 colonne della distanza (<i>gutter</i>) di 16px l'una</strong> (la scelta di 12 colonne consente di avere una flessibilità sufficiente per adattare il layout alle diverse dimensioni dello schermo o esigenze).

Di seguito è riportata una sintesi visiva del layout:

<img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/layout/Layout.png" alt="Layout generale di ARTISTA">

L'interfaccia si divide in due parti fondamentali: la <strong>view principale</strong> e la <strong>sidebar</strong>.
<img src="https://github.com/AsternoxCode/artista_design_system/blob/9d8764566972b2cb412d58c852ce795f82b59c33/layout/Layout-Padding.png" alt="Layout generale di ARTISTA, compreso di padding">


Ed hanno le seguenti caratteristiche:
<h4>View principale</h4>
  
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

<h4>Sidebar</h4>

```bash
W: 256px
H: 560px
Corner radius: 12px
Fill: Solid
#222222
```
<h4>Schede</h4>
  
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

<h3>Tipografia</h3>
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
