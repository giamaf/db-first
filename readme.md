# DB First
Modellizzo la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

---

Colonne|Tipo|Attributi
---|---|---
id| bigint | PRIMARY_KEY AUTO_INCREMENT
marca| VARCHAR | NOTNULL
modello| VARCHAR | NOTNULL
anno_immatricolazione | YEAR | NULL, DEFAULT('2023')
n.telaio | VARCHAR | UNIQUE, NOTNULL
alimentazione | CHAR | NOTNULL
cambio | CHAR | NOTNULL, DEFAULT('Manuale')
potenza | SMALLINT | NOTNULL, DEFAULT('1')
chilometraggio | CHAR | NOTNULL 
n.proprietari | TINYINT | NOTNULL, DEFAULT('1')
n.porte | CHAR | NULL, DEFAULT('3/5')
prezzo | CHAR | NOTNULL
paese | CHAR | NOTNULL, DEFAULT ('Italia')
cap | CHAR | NOTNULL