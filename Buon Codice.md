## Standard di Scrittura:

- Nomi della classe in maiuscolo usando il camel camel, Quindi maiuscole le prime lettere di ogni parola.
- I nomi dei metodo booleani di solito iniziano con 'is'.
- Nomi dei metodi e delle variabili prima lettera in minuscolo e poi sempre uso del camelcamel.
- Le variabili costanti tutto in maiuscolo e gli spazi si usa la '_'
- I nomi dei file o come i nomi delle classi che sarà come farò io o tutto in minuscolo e gli spazi con '_'

### Nomi variabili

- *Nomi delle classi*: Nomi per interi ma poche parole
- *Nomi dei metodi*: Comunemente dovrebbero essere verbi o che danno un senso di azione
- *Nomi delle variabili delle classi*: Dovrebbero essere sufficente scrivere la tipologia. Tipo se normalmente è restaurantModel dovrebbe bastere model o se è  widgetBuilder dovrebbe bastere buildler
- *Nomi delle variabili interne dei metodi*: Possono essere accorciate in modo molto snello tipo: colorScheme cls, texttheme tt

## Standard di progettazione:

- Uso del [Dash pattern](https://pub.dev/packages/dash) vedi [Medium](https://medium.com/flutter-community/announcing-dash-bloc-provider-made-easy-985f84a68f22)

## Standard delle directory:

- **data**: Dati dell'applicazione
- **generated**: File per il multilingua e il 'Provider' del Dash Pattern
- **interface**: Tutta l'interfaccia grafica, Widget
  - **page**: Widget utilizzati tramite BottomBar
  - **tab**: Widget utilizzati tramite TabBar
  - **screen**: Ogni schermata dell'applicazione
  - **view**: Widget che rappresentano in grafica un model
  - **widget**: Widget che rappresentano un layout e non dipendono da un modello
- **logic**: Tutta la logica dell'applicazione
  - **bloc**: File del Bloc/Dash Pattern
  - **altri file**: Database eo RestApi
- **model**: Modelli dell'applicazione
