# Konzeptionelle, technische und didaktische Überlegungen zu einem E-Portfolio für das lebensbegleitende Lernen

Vortrag am 21.10.2016 auf dem ÖZBF-Kongress in Salzburg

## Build the presentation

This presentation was built with Markdown, [Pandoc](http://pandoc.org/MANUAL.html#producing-slide-shows-with-pandoc) and [Reveal.js](http://lab.hakim.se/reveal-js/#/).

To build it yourself, install Reveal.js via `bower`

```bash
bower install reveal.js
```

Then type

```bash
pandoc -t revealjs -s main.md -o main.html -V revealjs-url=./bower_components/reveal.js -V theme=sky -V history=true -V controls=false -V css=style.css -V center=true -V transition=fade --slide-level=2
```

Open `main.html` in Google Chrome or Chromium.

## Developing with Live Reload

In order to (nearly) immediately preview what you write on a slide use a combination of two Atom packages:

- [atom-live-server](https://atom.io/packages/atom-live-server)
- [save-commands](https://atom.io/packages/save-commands)

The first package allows to open `main.html` with `localhost:3000` in Chrome while developing. Whenever `main.html` is changed, the file reloads and you get what you deserve.

Problem: You work on `main.md` and save it. You need to run the pandoc command shown above to change the file that's being shown in the browser, `main.html`. Thus, use the second package to run the command automatically when `main.md` was changed.

Hint: Place Atom to the left and Chrome on the right on your screen to avoid switching windows.


## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Namensnennung 4.0 International Lizenz</a>.
