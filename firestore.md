# Firestore

- [How to Structure Your Data](https://www.youtube.com/watch?v=haMOUb3KVSo) 
  - [More](https://firebase.google.com/docs/database/web/structure-data)
- [Write Information](https://angularfirebase.com/lessons/firestore-nosql-data-modeling-by-example/)
- [Plugin Utili](https://github.com/flutter/plugins/blob/master/FlutterFire.md)
- [Implementazione](https://firebase.google.com/docs/cloud-messaging/?authuser=3#implementation_paths)


## Regole

1. Documents have a limits - Documenti hanno un limite di lunghezza
2. You can't retrive partial document - Non puoi ritornare da query documenti parziali
3. Queries are shallow - Le quey sono lente
4. You are billed by the number of reads and writes you perform - Spendi soldi in base a quante letture e scritture fai
5. Query find document in collections - Le query cercano solo in una collezione di documenti
6. Array are weird - Gli array sono strani (altre traduzioni?)

## Standard

- Le collezioni, array o map vanno chiamati con nomi plurali, (_reviews, restaurants, types_)
- La tipologia dei nomi è la seguente (_restaurant_manager_), No camelCamel
- Da sinistra verso destra, categoria che raggruppa di più a categoria che ragruppa meno (_reviews_it, reviews_en, types_food_)

## Esempio Pratico

Abbiamo una serie di ristoranti

### Simple Restaurant Collection

App: Pagina Lista Ristoranti -> Pagina Dettaglio Ristorantea

| Restaurant | nome | rating |

### Restaurant and Review 

E le review? In una collezione dentro ad ogni documento. Path: /restaurant/<IdRestaurant>/review/<IdReview>

| Restaurant | nome | rating | _review_ |
- | Review | userId | rating | text | 


#### Review Problem

E se l'utente navigandando torna avanti e indietro dalla _pagina lista ristoranti_ alla _pagina dettaglio ristorante_?
- Scarichiamo ogni volta tutte le review del suddetto ristorante?... Per ora si, non so come sincronizzare i dati


