# Typography

A comprehensive guide to typography, featuring examples of global settings, headings, body text, lists, and various other elements.

<!-------------------- Fonts -------------------->

## Fonts

<!-- Font family -->

### Font family

`Inter` is used for FlyonUI docs. To change or customize this, consult the <a href="https://tailwindcss.com/docs/font-family" target="_blank" class="link link-primary">font-family</a> section in the TailwindCSS documentation.

<!-------------------- Font sizes -------------------->

## Font sizes

<!-- Headings -->

### Headings

Use of Tailwind CSS <a href="https://tailwindcss.com/docs/font-size" target="_blank" class="link link-primary">font size</a> utility classes to style various headings.

```html
<h1 class="text-base-content text-4xl">Heading 1</h1>
<h2 class="text-base-content text-3xl">Heading 2</h2>
<h3 class="text-base-content text-2xl">Heading 3</h3>
<h4 class="text-base-content text-xl">Heading 4</h4>
<h5 class="text-base-content text-lg">Heading 5</h5>
<h6 class="text-base-content text-base">Heading 6</h6>
```

<!-- Paragraph -->

### Paragraph

The `<p>` tag is extensively employed in HTML documents for composing longer passages of text, typically separated by blank lines. Adhering to proper usage of this tag can notably improve on-page SEO performance.

```html
<div>
  <h5 class="text-base-content text-lg font-semibold">Body text</h5>
  <p class="text-base-content/80 text-base">
    Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus. Duis
    mollis, est non commodo luctus.Duis mollis, est non commodo luctus.
  </p>
</div>
<div>
  <h5 class="text-base-content text-lg font-semibold">Small text</h5>
  <small class="text-base-content/80">
    Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus. Duis
    mollis, est non commodo luctus.Duis mollis, est non commodo luctus.
  </small>
</div>
<div>
  <h5 class="text-base-content text-lg font-semibold">Muted text</h5>
  <p class="text-base-content/50 text-base">
    Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus. Duis
    mollis, est non commodo luctus.Duis mollis, est non commodo luctus.
  </p>
</div>
```

<!-------------------- Semantic tags -------------------->

## Semantic tags

<!-- Inline text element-->

### Inline text elements

Styling for common inline HTML5 elements.

```html
<p class="text-base-content/80"> You can use the mark tag to <mark>highlight</mark> text. </p>
<p class="text-base-content/80"><del>This line of text is meant to be treated as deleted text.</del></p>
<p class="text-base-content/80"><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p class="text-base-content/80"><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p class="text-base-content/80"><u>This line of text will render as underlined.</u></p>
<p class="text-base-content/80"><small>This line of text is meant to be treated as fine print.</small></p>
<p class="text-base-content/80"><strong>This line rendered as bold text.</strong></p>
<p class="text-base-content/80"><em>This line rendered as italicized text.</em></p>
```

{{< table >}}
ELEMENT (TAG) |DESCRIPTION
`<mark>` | Used to highlight or mark text for emphasis or reference.
`<del>` | Indicates text that should be treated as deleted or removed from the document.
`<s>` | Represents text that is no longer relevant or accurate.
`<ins>` | Marks text that has been added to the document.
`<u>` | Renders text with an underline to indicate emphasis or annotation.
`<small>` | Denotes text that should be displayed in a smaller font size, often used for fine print or side comments.
`<strong>` | Renders text in a bold font to denote strong importance or emphasis.
`<em>` | Renders text in italics to indicate emphasis or stress.
{{< /table >}}

These HTML5 elements offer semantic significance to the content, effectively communicating specific intentions to both users and search engines.

<!-- Gradient text -->

<!-------------------- Misc -------------------->

## Misc

### Gradient text

Use the classes `bg-clip-text`, `text-transparent`, and `bg-gradient-{tw-utility-class}` to achieve a gradient overlay effect on a text element.

```html
<p class="bg-gradient-to-r from-primary to-error bg-clip-text text-transparent font-black text-4xl w-fit"> Gradient text </p>
```

<!-- First-line and first-letter -->

### First-line and first-letter

Apply styles to the initial line of a text block using the `::first-line` pseudo-element, and to the first letter with the `::first-letter` pseudo-element.

```html
<p class="first-letter:text-base-content text-justify first-letter:float-left first-letter:me-3 first-letter:text-7xl first-letter:font-bold first-line:uppercase first-line:tracking-widest" >
  You see this old vinyl record, weathered and worn, its label scratched and faded? At first glance, it may appear as
  nothing more than discarded junk. Yet, to me, it holds something infinitely precious—the sound of my childhood. It's
  not just music; it's a treasure trove of memories, each groove on its surface a testament to days gone by. As I gently
  place the needle onto its surface, I am transported back to a time when summer nights stretched on forever, filled
  with the warmth of family gatherings and pop that emanates from the speakers is like a whisper from the past, a
  nostalgic echo of moments I hold dear.
</p>
```

<!-- Open/closed state -->

### Open/closed state

Conditional application of styles based on the open state of either a `<details>` or `<dialog>` element.

```html
<div class="max-w-lg">
  <details class="open:bg-base-100 rounded-lg p-6 open:shadow" open>
    <summary class="text-base-content select-none text-base font-semibold">How did paperclips come to be?</summary>
    <div class="text-base-content/80 mt-3 text-base">
      <p>
        The humble paperclip has an interesting history. It was first patented in the late 19th century by Norwegian
        inventor Johan Vaaler, although the exact origin of the paperclip dates back even earlier to other similar
        designs.
      </p>
    </div>
  </details>
</div>
```


<!-- Text color -->
### Text color

Use these text color utilities to automatically apply the correct text color based on the background or border color. This ensures good contrast and readability across different components and themes.

<!-- Class Table -->
| Class | Type | Description |
| --- | --- | --- |
| text-bg-* | modifier | Utility class used to apply both text color and background color based on semantic color schemes. |
| text-bg-soft-* | modifier | Utility class used to apply both text color and a soft (lighter) background color using semantic color schemes. |
| text-border-* | modifier | Utility class used to apply both text color and border color using semantic color schemes. |


```html
<p class="text-bg-primary px-2 py-4"> This uses text-primary-content on a bg-primary background: <span class="font-medium">text-bg-primary</span> </p>

<p class="text-bg-soft-primary px-2 py-4"> This uses text-primary-content on a bg-soft-primary background: <span class="font-medium">text-bg-soft-primary</span> </p>

<p class="text-border-primary px-2 py-4"> This uses text-primary-content alongside a border-primary: <span class="font-medium">text-border-primary</span> </p>
```

<!-- Semantic gradient background -->
### Semantic gradient background

Use these semantic gradient background classes to create a smooth left-to-right gradient. The gradient starts with the semantic color on the left and transitions to a 20% darker shade on the right. This helps add depth and visual interest while maintaining consistency with your theme colors. 

<!-- Class Table -->
| Class | Type | Description |
| --- | --- | --- |
| gradient-bg | component | Base gradient background component that applies a neutral default gradient. |
| gradient-bg-primary | color | Applies a gradient background using the primary color scheme. |
| gradient-bg-secondary | color | Applies a gradient background using the secondary color scheme. |
| gradient-bg-accent | color | Applies a gradient background using the accent color scheme. |
| gradient-bg-info | color | Applies a gradient background using the info color scheme, typically used for informational highlights. |
| gradient-bg-success | color | Applies a gradient background using the success color scheme, often used to indicate positive status or confirmation. |
| gradient-bg-warning | color | Applies a gradient background using the warning color scheme, commonly used to indicate caution or attention. |
| gradient-bg-error | color | Applies a gradient background using the error color scheme, typically used to indicate errors or critical issues. |



```html
<span class="gradient-bg gradient-bg-primary w-full rounded-md p-5">
<p class="text-primary-content"> Use these semantic gradient background classes to create a smooth left-to-right gradient. The gradient starts with the semantic color on the left and transitions to a 20% darker shade on the right. This helps add depth and visual interest while maintaining consistency with your theme colors.
</p>
</span>
```
