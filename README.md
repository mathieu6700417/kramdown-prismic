# Kramdown Prismic

A Kramdown converter to convert documents into prismic rich text format.

## Status

*Very early*, still a proof of concept.

TODO:

- [x] heading1
- [x] heading2
- [x] heading3
- [x] heading4
- [x] heading5
- [x] heading6
- [x] paragraph
- [x] preformatted
- [x] strong
- [x] em
- [x] hyperlink
- [x] o-list-item
- [x] list-item
- [x] Image
- [ ] Embed

## Difference between markdown and rich text

| Markdown         | Prismic                    |
|------------------|----------------------------|
| Blockquote       | translated to preformatted |
| hr               | nothing                    |
| img              | moved to the top level     |
| nested list      | moved to the top level     |
| dl               | not supported              |
| dt               | not supported              |
| dd               | not supported              |
| table            | not supported              |
| thead            | not supported              |
| tobdy            | not supported              |
| tfoot            | not supported              |
| tr               | not supported              |
| td               | not supported              |
| math             | not supported              |
| footnote         | not supported              |
| entity           | Transformed to unicode     |
| typographic_sym  | Transformed to unicode     |
| smart_quote      |                            |
| abbreviation     | not supported              |
| html_element     | not supported              |
| xml_comment      | not supported              |
| xml_pi           | not supported              |
| comment          | not supported              |
| raw              |                            |

## Install

Not yet available on rubygems

## Usage

```ruby
require 'kramdown-prismic'

Kramdown::Document.new(markdown).to_prismic
```

## License

MIT
