- [Headings](#headings)
- [Collapsed sections](#organizing-information-with-collapsed-sections)
- [Links](#links)
- [Images](#images)
- [A table of contents](#a-table-of-contents)
- [Styling text](#styling-text)
- [Quoting text/Blockquotes](#quoting)
- [Tables](#tables)
- [Basic formatting syntax from GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Basic Syntax with best and bad practices](https://www.markdownguide.org/basic-syntax/)

### Headings

To create a heading, add one to six # symbols before your heading text. 
The number of # you use will determine the size of the heading.

```md
# The largest heading
## The second largest heading
###### The smallest heading
```

### Organizing information with collapsed sections

````
<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>
````

Result:
<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section.

You can add an image or a code block, too.

```ruby
puts "Hello World"
```
</details>

### Links

A relative link is a link that is relative to the current file. 
For example, if you have a `README` file in root of your repository, and you have another file in `docs/CONTRIBUTING.md`, 
and that `CONTRIBUTING.md` file contains `Reference` header,
the relative link to `Reference` section located in `CONTRIBUTING.md` in your `README` might look like this:
```
[Contribution guidelines for this project](docs/CONTRIBUTING.md#Reference)
```

### Images

You can display an image by adding `!` and wrapping the alt text in `[ ]`. Alt text is a short text equivalent of the information in the image. Then, wrap the link for the image in parentheses ().

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

### A table of contents
When you use two or more headings, GitHub automatically generates a table of contents which you can access by clicking
<svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-list-unordered" aria-label="The unordered list icon" role="img">
  <path fill-rule="evenodd" d="M2 4a1 1 0 100-2 1 1 0 000 2zm3.75-1.5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zM3 8a1 1 0 11-2 0 1 1 0 012 0zm-1 6a1 1 0 100-2 1 1 0 000 2z">
  </path>
</svg>
within the file header. 
Each heading title is listed in the table of contents and you can click a title to navigate to the selected section.

Alternatively you could create it manually with links. 
This option is useful when:
- you work with readme not only via browser and GitHub.
- in the file you only refer to the sections from other readme files.

### Styling text

| Example                                 | Output                                |
|:----------------------------------------|:--------------------------------------|
| `**Bold 1**`                            | **Bold 1**                            |
| `__Bold 2__`                            | __Bold 2__                            |
| `*Italic 1*`                            | *Italic 1*                            |
| `_Italic 2_`                            | _Italic 2_                            |
| `~~Strikethrough~~`                     | ~~Strikethrough~~                     |
| ``~~`Strikethrough code`~~``            | ~~`Strikethrough code`~~              |
| `**Bold and _nested italic_**`          | **Bold and _nested italic_**          |
| `***All bold and italic***`             | ***All bold and italic***             |
| `<sub>This is a subscript text</sub>`   | <sub>This is a subscript text</sub>   |
| `<sup>This is a superscript text</sup>` | <sup>This is a superscript text</sup> |

### Quoting 

Quoting text:

`> Text that is a quote`

Output:

> Text that is a quote

Quoting code:

Wrap value with a single \`: `quoted code`

Wrap multilines with \`\`\`:

```
cod line 1
code line 2
```


Wrap \`\`\` inside of quoted text, wrap it with 4 symbols \`\`\`\`:

````text
```
Some code
```
````






Strikethrough code wrap it with ``~~` `` and `` `~~``:

~~`Strikethrough code`~~

### Tables

By including colons `:` within the header row, you can define text to be left-aligned, right-aligned, or center-aligned:

```markdown
| Left-Aligned           |     Center Aligned     |          Right Aligned |
|:-----------------------|:----------------------:|-----------------------:|
| col 3 is               |    some wordy text     |                  $1600 |
| col 2 is               |        centered        |                    $12 |
| zebra stripes          |        are neat        |                     $1 |
| [tables link](#tables) | [tables link](#tables) | [tables link](#tables) |
```

Result:

| Left-Aligned           |     Center Aligned     |          Right Aligned |
|:-----------------------|:----------------------:|-----------------------:|
| col 3 is               |    some wordy text     |                  $1600 |
| col 2 is               |        centered        |                    $12 |
| zebra stripes          |        are neat        |                     $1 |
| [tables link](#tables) | [tables link](#tables) | [tables link](#tables) |

Note: In IntelliJ IDEA, you get a warning, if you do not format the value itself with the right number of spaces. 
Just apply the quick fix for the whole table.