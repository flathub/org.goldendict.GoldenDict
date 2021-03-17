# GoldenDict on Flathub

## How to run external translator programs?

You may want to call a external translator program as a dictionary source.

For instance, if you want to utilize [translate-shell](https://github.com/soimort/translate-shell) to provide Google Translate (default), Bing Translator, Yandex.Translate, or Apertium results, after installing `translate-shell` in your host system, add

- Enable: check
- Type: Plain Text
- Name: Gtrans EN-ES
- Command Line:
  ````shell
  flatpak-spawn --host trans -e google -s en -t es -show-original y -show-original-phonetics n -show-translation y -no-ansi -show-translation-phonetics n -show-prompt-message n -show-languages y -show-original-dictionary n -show-dictionary n -show-alternatives n "%GDWORD%"
  ````

to Dictionaries > Sources > Programs of GoldenDict. Note that you should adjust the language parameters according to your needs.
