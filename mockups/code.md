# Code

A code mockup displays code inside a styled box that mimics a code editor, making it perfect for showcasing code in documentation, demos, or tutorials.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| mockup-code | component | Container element. |


<!-------------------- Basic examples -------------------->

## Basic examples

<!-- Mockup code with line prefix -->

### Mockup code with line prefix

The `mockup-code` class is tailored to enhance the presentation of your code with a stylish layout. Use `data-prefix` to incorporate additional prefixes before text, such as `$`, `>`, or numeric indicators.

```html
<div class="mockup-code">
  <pre data-prefix="$"><code>npm i -D flyonui@latest</code></pre>
</div>
```

<!-- Multi line -->

### Multi line

Code spanning multiple lines.

```html
<div class="mockup-code">
  <pre data-prefix="$"><code>npm i -D flyonui@latest</code></pre>
  <pre data-prefix=">" class="text-warning"><code>installing...</code></pre>
  <pre data-prefix=">" class="text-success"><code>Done!</code></pre>
</div>
```

<!-- Highlighted line -->

### Highlighted line

Code example that highlights syntax.

```html
<div class="mockup-code">
  <pre data-prefix="1"><code>npm i -D flyonui@latest</code></pre>
  <pre data-prefix="2"><code>installing...</code></pre>
  <pre data-prefix="3" class="bg-warning text-warning-content"><code>Warning!</code></pre>
</div>
```

<!-- Scrollable body -->

### Scrollable body

Example of a scrollable code container.

```html
<div class="mockup-code">
  <pre data-prefix="~"><code>Magnam dolore beatae necessitatibus nemopsum itaque sit. Et porro quae qui et et dolore ratione.</code></pre>
</div>
```

<!-- Without prefix -->

### Without prefix

Example of code without a prefix.

```html
<div class="mockup-code">
  <pre><code>without prefix</code></pre>
</div>
```

<!-- Semantic color -->

### Semantic color

You can modify both the background and text colors.

```html
<div class="mockup-code bg-primary/20 text-primary rounded-xl">
  <pre><code>can be any color!</code></pre>
</div>
```
