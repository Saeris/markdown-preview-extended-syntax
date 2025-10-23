# Markdown Preview Extended

An extension pack which adds extended Markdown syntax support to VSCode's Markdown Preview. It's intended purpose is to ensure that what is rendered by the preview closely matches the HTML output one would get rendering the same document in a web application so that it can be styled using the same CSS for both.

## 📦 Contents

This is an extension pack consisting of the following VSCode Markdown Preview extensions. Where applicable, the usage syntax is provided as well as documentation about the associated semantic HTML element that is rendered.

Each extension runs the associated [markdown-it][markdown-it] plugin and the equivalent behavior can be achieved using [remark][remark] in JavaScript frameworks such as [Astro][astro] or [Nextjs][nextjs].

| syntax | html | extension | markdown-it | remark |
|:-:|:-:|-|-|-|
| `++insert++` | [`<ins>`][ins] | [Markdown Insert][vs-ins] | [markdown-it-ins][it-ins] | [remark-ins][re-ins] |
| `--delete--` | [`<del>`][del] | [Markdown Delete `<del>`][vs-ins] | [@saeris/markdown-it-del][it-del] | [@saeris/remark-del][re-del] |
| `==mark==` | [`<mark>`][mark] | [Markdown Mark][vs-mark] | [markdown-it-mark][it-mark] | [remark-flexible-markers][re-mark] |
| `[[ctrl]]` | [`<kbd>`][kbd] | [Markdown Keyboard `<kbd>`][vs-kbd] | [markdown-it-kbd][it-kbd] | [remark-kbd][re-kbd]* |
| `{本\|ほん}` |[`<ruby>`][ruby] | [Markdown DenDen Furigana][vs-ruby] | [markdown-it-ruby][it-ruby] | [remark-denden-ruby][re-ruby] |
| `31^st^` | [`<sup>`][sup] | [Markdown Superscript][vs-sup] | [@mdit/plugin-sup][it-sup] | [remark-supersub][re-sup] |
| `H~2~O` | [`<sub>`][sub] | [Markdown Subscript][vs-sub] | [@mdit/plugin-sub][it-sub] | [remark-supersub][re-sub] |
|` *[term]:` | [`<abbr>`][abbr] | [Markdown Abbreviation][vs-abbr] | [@mdit/plugin-abbr][it-abbr] | [remark-abbr][re-abbr] |
| `term`</br>`: def` | [`<dl>`][dl] | [Markdown Definition List `<dl>`][vs-dl] | [@mdit/plugin-dl][it-dl] | [remark-definition-list][re-dl] |
| `> [!NOTE]` | n/a | [Markdown GitHub Alerts][vs-alert] |[markdown-it-github-alerts][it-alert] | [remark-alerts][re-alert] | 
| `![](./img.svg)` | n/a | [Markdown Inline SVG][vs-svg] | [@saeris/markdown-it-inline-svg][it-svg] | [remark-inline-svg][re-svg] |
| n/a  | n/a | [Markdown Header Sections][vs-sec] | [markdown-it-header-sections][it-sec] | [remark-sectionize][re-sec] |

> \* requires additional configuration

## 🥂 License

Released under the [MIT license][license] © [Drake Costa][personal-website]

<!-- links -->

[markdown-it]: https://github.com/markdown-it/markdown-it
[remark]: https://github.com/remarkjs/remark
[astro]: https://astro.build/
[nextjs]: https://nextjs.org/
[license]: ./LICENSE.md
[personal-website]: https://saeris.gg

<!-- html elements -->
[ins]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/ins
[del]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/del
[mark]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/mark
[kbd]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/kbd
[ruby]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/ruby
[sup]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/sup
[sub]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/sub
[abbr]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/abbr
[dl]: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/dl

<!-- vscode extensions -->
[vs-alert]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-github-alerts
[vs-abbr]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-abbr
[vs-ins]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-ins
[vs-del]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-del
[vs-sup]: https://marketplace.visualstudio.com/items?itemName=DevHawk.markdown-sup
[vs-sub]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-subscript
[vs-mark]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-mark
[vs-kbd]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-keyboard
[vs-dl]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-definition-list
[vs-ruby]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-denden-furigana
[vs-svg]: https://marketplace.visualstudio.com/items?itemName=saeris.markdown-inline-svg
[vs-sec]: https://marketplace.visualstudio.com/items?itemName=Billaferd.vscode-header-sections

<!-- markdown-it plugins -->
[it-alert]: https://www.npmjs.com/package/markdown-it-github-alerts
[it-abbr]: https://www.npmjs.com/package/@mdit/plugin-abbr
[it-ins]: https://www.npmjs.com/package/markdown-it-ins
[it-del]: https://www.npmjs.com/package/@saeris/markdown-it-del
[it-sup]: https://www.npmjs.com/package/@mdit/plugin-sup
[it-sub]: https://www.npmjs.com/package/@mdit/plugin-sub
[it-mark]: https://www.npmjs.com/package/markdown-it-mark
[it-kbd]: https://www.npmjs.com/package/markdown-it-kbd
[it-dl]: https://www.npmjs.com/package/@mdit/plugin-dl
[it-ruby]: https://www.npmjs.com/package/markdown-it-ruby
[it-svg]: https://www.npmjs.com/package/@saeris/markdown-it-inline-svg
[it-sec]: https://www.npmjs.com/package/markdown-it-header-sections

<!-- remark plugins -->
[re-alert]: https://www.npmjs.com/package/remark-alerts
[re-abbr]: https://www.npmjs.com/package/remark-abbr
[re-ins]: https://www.npmjs.com/package/remark-ins
[re-del]: https://www.npmjs.com/package/@saeris/remark-del
[re-sup]:https://www.npmjs.com/package/remark-supersub
[re-sub]:https://www.npmjs.com/package/remark-supersub
[re-mark]: https://github.com/ipikuka/remark-flexible-markers
[re-kbd]: https://www.npmjs.com/package/remark-kbd
[re-dl]: https://www.npmjs.com/package/remark-definition-list
[re-ruby]: https://www.npmjs.com/package/remark-denden-ruby
[re-svg]: https://www.npmjs.com/package/remark-inline-svg
[re-sec]: https://www.npmjs.com/package/remark-sectionize
