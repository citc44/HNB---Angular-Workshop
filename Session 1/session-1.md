# Session 1

A deep dive to various frontend technology that are widely used in the industries, starting with little history of web development how it emerge to overwhelming SDKs and tools.


>## History
1. Static Content [ 1990 to 1995 ]
2. Dynamic Content [ 1995 to 2002 ] 
3. Dynamic **Content** and Interactive UI [ 2002 to 2007 ]
4. Dynamic ~~`Content`~~ ***Data*** to **UI** [ 2007 to 2020 ]
    *   UI Design - Graphics
    *   **UI Development - Programming** <---*This is what we are going to learn with Angular*
  

![Images](/images/web-history.jpg)

>## UI Design / Graphics
1. Photoshop - Layout / Image / Graphics / Concept
2. CSS [ Cascading Style Sheet ] - Implementation of above.

**Preprocessor**

1. LESS [ [Leaner Style Sheets](http://lesscss.org/) ] - Javascipt based
2. SASS [ [Syntactically awesome style sheets ](https://sass-lang.com/) - Ruby based ]
3. SCSS [ SASSy CSS ]

```
SCSS / SASS / LESS === Tranforms To ===> CSS
```
>###  CSS EXAMPLE - Two body size with exactly half size table.

```CSS
.body { width: 200; } /* Small body*/
.table {  width: 100; } /* Half the table size */

.body-large { width: 400; } /* Double of  Large Body */
.table-large { width: 200; } /* Half of the large body size*/
```

>###  SCSS EXAMPLE - Two body size with exactly half size table.

```SCSS
$body: 200;
.body: { width: $body; }            //  Generates .body { width: 200; }
.table: {width: $body / 2; }        // .table {  width: 100; }
.body-large { width: $body * 2; }   // .body-large { width: 400; }
.table-large { width: $body; }      // .table-large { width: 200; }
```