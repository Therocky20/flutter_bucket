## Configure Flutter

1. [Follow the guide](https://flutter.dev/docs/get-started/install)
2. **Very Important:** `flutter doctor` helps you a lot, follow what is required step by step
3. _Optional:_ [For more plugin for your Ide](IntelliJ%20Plugins)

## Start Code: Basic Guide

- 'const' E' molto **importante!!**
    1. Cosa fa? Salva in una speciale HashMap l'oggetto segnato dal _const_: const SizedBox(height: 16.0)
    2. Come risparmia RAM? Se un oggetto contrassegnato con _const_ viene inizializzato viene prima controllato se esiste già nell HashMap.
        - In caso positivo viene preso l'oggetto già esistente
        - In caso negativo viene creato e salvato nell'HashMap
    3. Cosa non permette di fare? Tutti gli oggetti marcati const non possono essere modificati in alcun modo    
- L'architettura base per il tuo codice [BLoC](https://www.didierboelens.com/2018/08/reactive-programming---streams---bloc/)
    - [ReactiveConf 2018 - Brian Egan & Filip Hracek: Practical Rx with Flutter](https://www.youtube.com/watch?v=7O1UO5rEpRc)
    - [More Information](https://medium.com/flutterpub/effective-bloc-pattern-45c36d76d5fe)
- La migliore archittettura per il tuo codice [Dash](https://medium.com/flutter-community/announcing-dash-bloc-provider-made-easy-985f84a68f22)
- **Prima di iniziare** [Un semplice esercizio](https://medium.com/flutter-community/flutter-bloc-with-streams-6ed8d0a63bb8)
- Utilizza la classe [Theme](https://medium.com/@mx_tino/flutter-themes-9cebc0fecd1d) per la tua App
- Che style ha la tua App? Material Design, ovviamente!:
  - [Guida](https://material.io/design/color/#color-usage-palettes)
  - [ColorScheme](https://api.flutter.dev/flutter/material/ColorScheme-class.html) la classe che definisce i colori della tua
  - [Tools](https://material.io/tools/color/#!/?view.left=0&view.right=0)
- [StatefulWidget - Ciclo di Vita](https://flutterbyexample.com/stateful-widget-lifecycle/#4-didChangeDependencies)

## More Utility

- [Flutter Awesome](https://github.com/Solido/awesome-flutter/blob/master/README.md)
- [Plugins Utili](https://github.com/BreX900/flutter_bucket/blob/master/plugins_flutter.md)
- [Altre linee guida](https://github.com/BreX900/flutter_bucket/blob/master/Buon%20Codice.md)
- [GitHub](https://github.com/) Utlizza questo servizio per salvare in cloud il tuo progetto e per poterlo condividere in caso di necessità

## Altro di poca rilevanza

- [Internationalization Tutorial](https://medium.com/@datvt9312/flutter-internationalization-tutorials-part-2-intl-package-approach-and-as-plugin-approach-b0aabdb254d8)
- [WordPress REST APi](https://github.com/BreX900/flutter_bucket/blob/master/WordPress%20REST%20Api.md)
