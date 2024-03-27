# CSS GRID


## grid-template-columns & grid-template-rows

```css
/* Slouží k definování sloupců */
.class {
   grid-template-columns: 1fr 1fr;
}


/* Slouží k definování řádků, pokud není nutné lepší nepoužívat
   Přináší mnohdy zbytečnou komplexitu */
.class {
   grid-template-row: 1fr;
}
```

- grid columns se na výšku roztahují podle nejvyššího contentu, pokud content nevycentrujeme nebo jinak umístíme, mají sloupce jednotlivý sloupce výšku fit-content

## grid-column & grid-row

```css
/* Zkratka pro grid-column-start a grid-column-end,
 první hodnota je pro start a oděluje se / , definuje umístění elementu v mřížce */
.class {
  grid-column: 1 / 3;
}


/* To samé jako pro grid-column akorát místo sloupců se počítají řádky */
.class {
  grid-row: 1 / 3;
}
```
### tipy a triky s vlastností grid-column

```css
/* Zabere vždy všechny sloupce v řádku */
.class {
  grid-column: 1 / -1;
}


/* Funguje pouze částečně, ve firefoxu není podporován, lepší nepoužívat */
.class {
  grid-row: 1 / -1;
}

/* Hodnota za klíčovým slovem span zabere počet sloupců */
.class {
  grid-column: span 2; /*zabere dva sloupce*/
}
```

## Podklady

[CSS TRICKS](https://css-tricks.com/snippets/css/complete-guide-grid/)

[Vzhuru dolů](https://www.vzhurudolu.cz/prirucka/css-grid)

[Gird garden](https://cssgridgarden.com/#cs)
