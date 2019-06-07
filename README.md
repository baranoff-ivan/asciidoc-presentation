# HOWTO
1. Clone this repository.
2. Prepare your slides in AsciiDoc format ([AsciiDoc syntax](https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/), [Asciidoctor Reveal.js](https://asciidoctor.org/docs/asciidoctor-revealjs/#syntax-examples))
3. Clone reveal.js presentation framework to the repository folder:
  ```sh
  git clone -b 3.8.0 --depth 1 https://github.com/hakimel/reveal.js.git
  ```
3. Generate HTML presentation from the AsciiDoc source:
  ```sh
  sh generate.sh CONTENT_FILE.adoc
  ```
4. Publish your presentation to localhost:
  ```sh
  python3 -m http.server 8000
  ```
5. Open your presentation at http://localhost:8000.

# Additional info
* To enable AsciiDoc syntax highlighting in vim use [vim-asciidoctor](https://github.com/habamax/vim-asciidoctor).
