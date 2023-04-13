# GoldenDict on Flathub

## How to use the translator program `translate-shell`?

You can use the [translate-shell](https://github.com/soimort/translate-shell) translator program as a dictionary source. It will return results from Google Translate (default), Bing Translator, Yandex.Translate or Apertium.

Translate-shell is bundled with this Flatpak. To use it in addition to the default dictionary sources, go to Dictionaries > Sources > Programs of GoldenDict, and add an item with the following settings


- Enable: check
- Type: Plain Text
- Name: Gtrans EN-ES
- Command Line:
  ````shell
  trans -engine google -source en -target es -show-original y -show-original-phonetics n -show-translation y -no-ansi -show-translation-phonetics n -show-prompt-message n -show-languages y -show-original-dictionary n -show-dictionary n -show-alternatives n "%GDWORD%"
  ````

Note that you should adjust the language parameters according to your needs, according to [its documentation](https://www.soimort.org/translate-shell/#usage).
