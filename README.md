### Importa la collection di esempio fornita in un database dedicato.<br>Esegui le seguenti query usando MongoCompass e prendi nota delle query che hai usato e il numero delle risorse trovate.

1. trova tutte le risorse con il dato isActive corrispondente a true
   <br>{isActive : true}

2. trova tutte le risorse con il dato age maggiore di 26
   <br>{age : { $gt:26}}

3. trova tutte le risorse con il dato age maggiore di 26 e minore o uguale a 30
   <br>{age : {$gt:26, $lte:30}}

4. trova tutte le risorse con il dato eyes che sia brown o blue
   <br>{eyeColor : {$in : ["brown", "blue"]}}

5. trova tutte le risorse che non presentano il dato eyes uguale a grren
   <br>{eyeColor : {$ne: "green"}}

6. trova tutte le risorse con non presentano il dato eyes uguale a green e neanche blue
   <br>{eyeColor : {$nin: ["green", "blue"]}}

7. trova tutte le risorse con il dato company uguale a "FITCORE" e ritorna solo l'email
   <br>{company : "FITCORE"}<br>project {emeil : 1}
