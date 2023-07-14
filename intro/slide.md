---
theme: default
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://img.freepik.com/fotos-premium/natuerlicher-quadratischer-weisser-hintergrund_476151-596.jpg')
marp: true
footer: 'https://github.com/ottafregu/ecommerce-freguglia-dolcini'
header: '**Carlotta Freguglia** _immagine di impresa_'
---

# Presentazione del mio e-commerce

_**Corso di WebDesign 2**_

A. A. 2022-2023


<!-- _paginate: false -->
<!-- _footer: "" -->
<!-- style: "
img[alt~='center'] {
  display: block;
  margin: 0 auto;
}

header{
  font-family: 'DM Serif Display', serif;
}
" -->

---

## Aree di lavoro

Per questo progetto ho creato un sito e-commerce sulla vendita di dolci, composto da
**4 pagine collegate tra di loro:** 
- Home
- Pagina prodotto
- Carrello
- About us

Queste pagine sono accomunate da una **headline** e da un **footer** ricorrenti in ogni pagina.
![gatto h:50px ](/img/sfondosito.png)


---

# Elementi comuni

_Headline & Footer_

---

## Headline

Nella parte sinistra della headline troviamo un **menù a comparsa** che, al click sulle tre lineette, richiama l'evento 'activateMenu', permettendo così alle 3 fasce '.menu-top', '.menu-middle' e '.menu-bottom' di espandersi e rendendo così visibile sia il loro link interno '.menu-text', sia la X '.menu-close' per chiudere l'intero menù e farlo tornare alla forma iniziale.

---

## Headline

Al centro della headline troviamo il **logo del brand** che funge anche da collegamento alla home del sito.

---

## Headline

Nella parte destra della headline trviamo il **carrello** in cui, grazie alla funzione 'aggiungiAlCarrello' e 'rimuoviDalCarrello' associate ai tasti presenti sotto ai prodotti, possiamo vedere il numero di questi inseritovi dentro.
Inoltre, questa icona funge da collegamento alla pagina del carrello stesso.

---

## Footer

Nel footer troviamo la mappa, i contatti e i social: **tre elementi inline** che, allo stringersi della pagina, si posizionano uno sotto l'altro grazie ad una **media query**.

---

# Pagine singole

_Home - Prodotto - Carrello - About us_

---

## Home page

Nella home page troviamo uno slider, un teitolo e le tre caselle prodotto.
- Lo slider, cui codice nativo è stato preso da https://swiperjs.com/, contiene 6 immagini di dolci che scorrono una dopo l'altra grazie alla funzione Javascript 'autoplay'.

- Sotto allo slider vi è un titlo che funziona da collegamento con un'ancora interna alla pagina, posizionata appena sopra, che permette al click sulla scritta di far salire la pagina, in modo da rendere visibili le tre caselle prodotto.

---

## Home page

- Sotto alla scitta ci sono le tre caselle prodotto che, usando la class 'card h-100', contengono l'immagine del prodotto, il suo nome, la descrizione, il costo e i tasti collegati al carrello per aggiungere o togliere quantità.

Al passaggio del puntatore sulle immagini dei prodotti, queste diminuiscono l'opacità e si crea un'ombra marrone attorno ad esse. Cliccandoci su invece, si viene reindirizzati alla pagine del prodotto stesso.

---

## Pagina prodotto 

Nella pagina prodotto troviamo un container fluido di boostrap, contenente due colonne in cui è inserita nuovamente la foto del prodotto e le informazioni a riguardo.

Il box si presenta bianco con un'ombra marrone all'esterno; nella parte delle informazioni sono presenti dei menù a tendina il cui codice nativo è stato preso da https://getbootstrap.com/, che permettono di scegliere quella che sarà la personalizzazione del prodotto.

---

## Carrello 

Cliccando nella parte di menù riguardante o nell'icona in alto a destra, veniamo rimandati alla pagina carrello. Qui troviamo sempre un container fluido come prima, ma con più righe e colonne.
Al suo interno sono riportati l'immagine del prodotto, il suo costo, la quantità che desideriamo (grazie ad una casella di testo editabile), il prezzo totale  e la presenza o meno di personalizzazioni.

---

## Carrello

Aumentando la quantità di prodotto desiderato, si attiverà una funzione di calcolo 'updateCosts' che aggiornernerà il costo totale del prodotto moltiplicando il costo base per la quantità inserita.
Inoltre sommerà i costi totali dei vari prodotti presenti nel carrello per avere un subtotale 'subTotal', visibile nella riga **Totale prodotti**, per poi aggiungergli i costi di spedizione 'shippingCost' e aggiornare così il costo totale 'grandTotal' visibile nella riga **Totale**.

---

## About us 

Il corpo della pagina _**chi siamo**_ è diviso in 3 grandi fasce, riconoscibili dal distacco delle immagini di sfondo che ricoprono la larghezza dell'intera fascia:
- Nella prima troviamo un titolo in alto al centro e un box con testo posizionato basso al centro, grazie al tag "vertical-align: bottom"
- Nella seconda troviamo un box con opacità dell'80%, posizionato in alto a sinistra e contenente sia un titolo h2 che un testo
- Nella terza troviamo un box posizionato al centro e contenente del testo, con al di sotto un bottone di rimando alla homepage

---

# Responsive delle pagine

_Adattmenti creati grazie alle **media query**_

---

## Home page

_Adattmenti creati grazie alle **media query**_

---