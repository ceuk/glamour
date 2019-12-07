# Gold Style Reference

## document

The `document` element represents the markdown's body.

### Attributes

| Attribute        | Value  | Description                                           |
| ---------------- | ------ | ----------------------------------------------------- |
| prefix           | string | Printed before the first element during rendering     |
| suffix           | string | Printed after the last element during rendering       |
| indent           | number | Specifies the indentation of the document             |
| margin           | number | Specifies the margin around the document              |
| color            | color  | Defines the default text color for the document       |
| background_color | color  | Defines the default background color for the document |

### Example

```
"document": {
    "indent": 2,
    "background_color": "234",
    "prefix": "\n",
    "suffix": "\n"
}
```

## paragraph

The `paragraph` element represents a paragraph in the document.

### Attributes

| Attribute        | Value  | Description                                         |
| ---------------- | ------ | --------------------------------------------------- |
| prefix           | string | Printed before the first element in a paragraph     |
| suffix           | string | Printed after the last element in a paragraph       |
| indent           | number | Specifies the indentation of paragraphs             |
| margin           | number | Specifies the margin around paragraphs              |
| color            | color  | Defines the default text color for paragraphs       |
| background_color | color  | Defines the default background color for paragraphs |

### Example

```
"paragraph": {
    "margin": 4,
    "color": "15",
    "background_color": "235"
}
```

## heading

The `heading` element represents a heading.

## h1 - h6

The `h1` to `h6` elements represent headings. `h1` defines the most important
heading, `h6` the least important heading. Undefined attributes are inherited
from the `heading` element.

### Attributes

| Attribute        | Value  | Description                                       |
| ---------------- | ------ | ------------------------------------------------- |
| prefix           | string | Printed before a heading                          |
| suffix           | string | Printed after a heading                           |
| indent           | number | Specifies the indentation of headings             |
| margin           | number | Specifies the margin around headings              |
| color            | color  | Defines the default text color for headings       |
| background_color | color  | Defines the default background color for headings |
| bold             | bool   | Increases text intensity                          |
| faint            | bool   | Decreases text intensity                          |
| italic           | bool   | Prints the text in italic                         |
| crossed_out      | bool   | Enables strikethrough as text decoration          |
| underline        | bool   | Enables underline as text decoration              |
| overlined        | bool   | Enables overline as text decoration               |
| blink            | bool   | Enables blinking text                             |
| conceal          | bool   | Conceals / hides the text                         |
| inverse          | bool   | Swaps fore- & background colors                   |

### Example

```
"heading": {
    "prefix": "\n",
    "margin": 4,
    "color": "15",
    "background_color": "57"
},
"h1": {
    "prefix": "\n=> ",
    "suffix": " <=",
    "margin": 2,
    "bold": true,
    "background_color": "69"
},
"h2": {
    "prefix": "\n# "
}
```

## text

The `text` element represents a block of text.

### Attributes

| Attribute        | Value  | Description                                           |
| ---------------- | ------ | ----------------------------------------------------- |
| prefix           | string | Printed before a text gets printed                    |
| suffix           | string | Printed after a text got printed                      |
| color            | color  | Defines the default text color for the document       |
| background_color | color  | Defines the default background color for the document |
| bold             | bool   | Increases text intensity                              |
| faint            | bool   | Decreases text intensity                              |
| italic           | bool   | Prints the text in italic                             |
| crossed_out      | bool   | Enables strikethrough as text decoration              |
| underline        | bool   | Enables underline as text decoration                  |
| overlined        | bool   | Enables overline as text decoration                   |
| blink            | bool   | Enables blinking text                                 |
| conceal          | bool   | Conceals / hides the text                             |
| inverse          | bool   | Swaps fore- & background colors                       |

### Example

```
"text": {
    "bold": true,
    "color": "15",
    "background_color": "57"
}
```

## list

The `list` element represents a list in the document.

### Attributes

| Attribute        | Value  | Description                                    |
| ---------------- | ------ | ---------------------------------------------- |
| prefix           | string | Printed before a list                          |
| suffix           | string | Printed after a list                           |
| indent           | number | Specifies the indentation of lists             |
| margin           | number | Specifies the margin around lists              |
| color            | color  | Defines the default text color for lists       |
| background_color | color  | Defines the default background color for lists |

### Example

```
"list": {
    "margin": 4,
    "color": "15",
    "background_color": "52"
}
```

## item

The `item` element represents an item in lists.

### Attributes

| Attribute        | Value  | Description                                    |
| ---------------- | ------ | ---------------------------------------------- |
| prefix           | string | Printed before an item                         |
| suffix           | string | Printed after an item                          |
| color            | color  | Defines the default text color for items       |
| background_color | color  | Defines the default background color for items |
| bold             | bool   | Increases text intensity                       |
| faint            | bool   | Decreases text intensity                       |
| italic           | bool   | Prints the text in italic                      |
| crossed_out      | bool   | Enables strikethrough as text decoration       |
| underline        | bool   | Enables underline as text decoration           |
| overlined        | bool   | Enables overline as text decoration            |
| blink            | bool   | Enables blinking text                          |
| conceal          | bool   | Conceals / hides the text                      |
| inverse          | bool   | Swaps fore- & background colors                |

### Example

```
"item": {
    "prefix": "• "
}
```

## enumeration

The `enumeration` element represents an item in ordered lists.

### Attributes

| Attribute        | Value  | Description                                    |
| ---------------- | ------ | ---------------------------------------------- |
| prefix           | string | Printed before an item                         |
| suffix           | string | Printed after an item                          |
| color            | color  | Defines the default text color for items       |
| background_color | color  | Defines the default background color for items |
| bold             | bool   | Increases text intensity                       |
| faint            | bool   | Decreases text intensity                       |
| italic           | bool   | Prints the text in italic                      |
| crossed_out      | bool   | Enables strikethrough as text decoration       |
| underline        | bool   | Enables underline as text decoration           |
| overlined        | bool   | Enables overline as text decoration            |
| blink            | bool   | Enables blinking text                          |
| conceal          | bool   | Conceals / hides the text                      |
| inverse          | bool   | Swaps fore- & background colors                |

### Example

```
"enumeration": {
    "prefix": ". "
}
```

## link

The `link` element represents a link.

### Attributes

| Attribute        | Value  | Description                                    |
| ---------------- | ------ | ---------------------------------------------- |
| prefix           | string | Printed before the link                        |
| suffix           | string | Printed after the link                         |
| color            | color  | Defines the default text color for links       |
| background_color | color  | Defines the default background color for links |
| bold             | bool   | Increases text intensity                       |
| faint            | bool   | Decreases text intensity                       |
| italic           | bool   | Prints the text in italic                      |
| crossed_out      | bool   | Enables strikethrough as text decoration       |
| underline        | bool   | Enables underline as text decoration           |
| overlined        | bool   | Enables overline as text decoration            |
| blink            | bool   | Enables blinking text                          |
| conceal          | bool   | Conceals / hides the text                      |
| inverse          | bool   | Swaps fore- & background colors                |

### Example

```
"link": {
    "color": "123",
    "underline": true,
    "prefix": "(",
    "suffix": ")"
}
```

## link_text

The `link_text` element represents the text associated with a link.

### Attributes

| Attribute        | Value  | Description                                       |
| ---------------- | ------ | ------------------------------------------------- |
| prefix           | string | Printed before the text                           |
| suffix           | string | Printed after the text                            |
| color            | color  | Defines the default text color for the text       |
| background_color | color  | Defines the default background color for the text |
| bold             | bool   | Increases text intensity                          |
| faint            | bool   | Decreases text intensity                          |
| italic           | bool   | Prints the text in italic                         |
| crossed_out      | bool   | Enables strikethrough as text decoration          |
| underline        | bool   | Enables underline as text decoration              |
| overlined        | bool   | Enables overline as text decoration               |
| blink            | bool   | Enables blinking text                             |
| conceal          | bool   | Conceals / hides the text                         |
| inverse          | bool   | Swaps fore- & background colors                   |

### Example

```
"link_text": {
    "color": "123",
    "bold": true
}
```

## image

The `image` element represents an image.

### Attributes

| Attribute        | Value  | Description                                     |
| ---------------- | ------ | ----------------------------------------------- |
| prefix           | string | Printed before an image                         |
| suffix           | string | Printed after an image                          |
| color            | color  | Defines the default text color for images       |
| background_color | color  | Defines the default background color for images |
| bold             | bool   | Increases text intensity                        |
| faint            | bool   | Decreases text intensity                        |
| italic           | bool   | Prints the text in italic                       |
| crossed_out      | bool   | Enables strikethrough as text decoration        |
| underline        | bool   | Enables underline as text decoration            |
| overlined        | bool   | Enables overline as text decoration             |
| blink            | bool   | Enables blinking text                           |
| conceal          | bool   | Conceals / hides the text                       |
| inverse          | bool   | Swaps fore- & background colors                 |

### Example

```
"image": {
    "color": "123",
    "prefix": "[Image: ",
    "suffix": "]"
}
```

## image_text

The `image_text` element represents the text associated with an image.

### Attributes

| Attribute        | Value  | Description                                       |
| ---------------- | ------ | ------------------------------------------------- |
| prefix           | string | Printed before the text                           |
| suffix           | string | Printed after the text                            |
| color            | color  | Defines the default text color for the text       |
| background_color | color  | Defines the default background color for the text |
| bold             | bool   | Increases text intensity                          |
| faint            | bool   | Decreases text intensity                          |
| italic           | bool   | Prints the text in italic                         |
| crossed_out      | bool   | Enables strikethrough as text decoration          |
| underline        | bool   | Enables underline as text decoration              |
| overlined        | bool   | Enables overline as text decoration               |
| blink            | bool   | Enables blinking text                             |
| conceal          | bool   | Conceals / hides the text                         |
| inverse          | bool   | Swaps fore- & background colors                   |

### Example

```
"image_text": {
    "color": "8"
}
```

## code_block

The `code_block` element represents a block of code.

### Attributes

| Attribute        | Value  | Description                                           |
| ---------------- | ------ | ----------------------------------------------------- |
| prefix           | string | Printed before a code block                           |
| suffix           | string | Printed after a code block                            |
| indent           | number | Specifies the indentation of code blocks              |
| margin           | number | Specifies the margin around code blocks               |
| theme            | string | Defines the chroma theme used for syntax highlighting |
| color            | color  | Defines the default text color for code blocks        |
| background_color | color  | Defines the default background color for code blocks  |

### Example

```
"code_block": {
    "margin": 4,
    "color": "200",
    "theme": "solarized-dark"
}
```

## table

The `table` element represents a table of data.

### Attributes

| Attribute        | Value  | Description                                     |
| ---------------- | ------ | ----------------------------------------------- |
| prefix           | string | Printed before a table                          |
| suffix           | string | Printed after a table                           |
| indent           | number | Specifies the indentation of tables             |
| margin           | number | Specifies the margin around tables              |
| color            | color  | Defines the default text color for tables       |
| background_color | color  | Defines the default background color for tables |

### Example

```
"table": {
    "margin": 4
}
```

## hr

The `hr` element represents a horizontal rule.

### Attributes

| Attribute        | Value  | Description                                                  |
| ---------------- | ------ | ------------------------------------------------------------ |
| prefix           | string | Printed before the horizontal rule                           |
| suffix           | string | Printed after the horizontal rule                            |
| color            | color  | Defines the default text color for the horizontal rule       |
| background_color | color  | Defines the default background color for the horizontal rule |
| bold             | bool   | Increases text intensity                                     |
| faint            | bool   | Decreases text intensity                                     |
| italic           | bool   | Prints the text in italic                                    |
| crossed_out      | bool   | Enables strikethrough as text decoration                     |
| underline        | bool   | Enables underline as text decoration                         |
| overlined        | bool   | Enables overline as text decoration                          |
| blink            | bool   | Enables blinking text                                        |
| conceal          | bool   | Conceals / hides the text                                    |
| inverse          | bool   | Swaps fore- & background colors                              |

### Example

```
"hr": {
    "prefix": "---"
}
```


## block_quote
## emph
## strong
## del
## html_block
## softbreak
## hardbreak
## code
## html_span