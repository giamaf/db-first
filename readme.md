# DB First
Modellizzo la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

---

Colonne|Tipo|Attributi
---|---|---
id| BIGINT | PRIMARY_KEY, AUTO_INCREMENT
marca| VARCHAR(20) | NOTNULL
modello| VARCHAR(30) | NOTNULL
anno_immatricolazione | DATE | NOTNULL, DEFAULT('2023')
n.telaio | CHAR(17) | UNIQUE, NOTNULL
alimentazione | CHAR | NOTNULL
cambio | CHAR | NOTNULL, DEFAULT('Manuale')
potenza | SMALLINT | NOTNULL, DEFAULT('1')
chilometraggio | MEDIUMINT | NOTNULL
n.proprietari | TINYINT | NOTNULL, DEFAULT('1')
n.porte | CHAR | NULL, DEFAULT('3/5')
prezzo | FLOAT(9,2) | NULL
paese | CHAR | NOTNULL, DEFAULT ('Italia')
cap | CHAR | NOTNULL