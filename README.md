
# Python Hackathon Entry Task <br>(2017-06-17)

Intro úloha na hackathon: **Generátor a verifikátor rodného čísla** 

Program **birthnumber.py** bude pracovať v 2 módoch - buď bude generovať nové rodné číslo (žiaden argument) alebo bude verifikovať poskytnuté číslo z príkazového riadku (1 argument).

Podmienky na generovanie a overenie rodného čísla sú nasledovné:
 * číslo musí obsahovať 10 čisel (pre ľudí, ktorí sa narodili po roku 1954)
 * alebo musí osahovať 9 čisel (pre ľudí, ktorí sa narodili do roku 1953)
 * číslo má 2 časti - dátum narodenia a kontrolný súčet (CCCC) v tvare YYMMDD/CCCC
 * celé číslo musí byť delitelné číslom 11
 * ženy majú v mesiaci narodenia pridanú hodnotu 50

### Príklad: 
**861107/2239** je validné rodné číslo pre muža, ktorý sa narodil 7.11.1986. <br>**025226/1306** je validné rodné číslo ženy narodenej 26.02.2002.

Pre spustenie overenia rodného čísla použijeme príkaz: 

     $ birthnumber.py YYMMDD/CCCC
     
kde `YYMMDD/CCCC` je konkrétne rodné číslo, ktoré chceme overiť. 

Očakávaný výstup v prípade nesprávneho rodného čísla je hláška s chybami, ktoré počas validácie nastali. <br>Príklad:

     Provided birth number is INVALID.
     <reason>
     <another-reason>

Pre generovanie to bude interaktívny proces:
     
     $ birthnumber.py

výstup:

    Day of the birth [YYYY-MM-DD]: <user input>
    Sex [M/F]: <user input>
    Generated birth number: YYMMDD/CCCC

Pre implementáciu použite **Python 3**. Nie je nutné zasielať nám riešenie, je to pre vaše posúdenie či by ste zvládli podobné a náročnejšie typy úloh na hackathone.<br>
V prípade ďaších informácií nás môžte kontaktovať na tech@engeto.com
