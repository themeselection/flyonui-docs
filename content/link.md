# Link

The link component facilitates setting hyperlinks from inline text items, buttons, or cards to navigate between pages or external websites.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| link | component | Adds underline to a text. |
| link-hover | style | Only show underline on hover. |
| link-animated | style | Show underline on hover with animation. |
| link-neutral | color | Applies'neutral' color to link. |
| link-primary | color | Applies'primary' color to link. |
| link-secondary | color | Applies'secondary' color to link. |
| link-accent | color | Applies'accent' color to link. |
| link-success | color | Applies'success' color to link. |
| link-info | color | Applies'info' color to link. |
| link-warning | color | Applies'warning' color to link. |
| link-error | color | Applies'error' color to link. |


<!-------------------- Variants -------------------->

## Variants

<!-- Default -->

### Default

The `link` component class serves as the standard class for the basic anchor tag.

```html
<a href="#" class="link">Default link</a>
```

<!-- Underline on hover -->

### Underline on hover

Apply the `link-hover` modifier class to make links underlined when hovered over.

```html
<a href="#" class="link link-hover">Underline when hovered over.</a>
```

<!-- Animated underline -->

### Animated underline

Apply the `link-animated` modifier class to make links underlined with animation on hovered over.

```html
<a href="#" class="link link-animated"> Animated underline when hovered over.</a>
```

> **Info:** The modifier classes `link-animated` and `link-hover` are also applicable to semantic links.

<!-------------------- Colors -------------------->

## Colors

<!-- Semantic links -->

### Semantic links

Utilize the `link-{semantic-color}` modifier class to assign specific semantic colors to links.

```html
<a href="#" class="link link-neutral">Neutral link</a>
<a href="#" class="link link-primary">Primary link</a>
<a href="#" class="link link-secondary">Secondary link</a>
<a href="#" class="link link-accent">Accent link</a>
<a href="#" class="link link-info">Info link</a>
<a href="#" class="link link-success">Success link</a>
<a href="#" class="link link-warning">Warning link</a>
<a href="#" class="link link-error">Error link</a>
```

<!-- Custom Color -->

### Custom Color

Use the `--link-color` for the custom color of the link.

```html
<a href="#" class="link [--link-color:purple]">Default</a>
<a href="#" class="link link-hover [--link-color:purple]">Underline on Hover</a>
<a href="#" class="link link-animated [--link-color:purple]">Animated Underline</a>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- In paragraphs -->

### In paragraphs

Below is an example demonstrating how to use links within paragraph.

```html
<p>Tailwind CSS resets the appearance of links by default.<br/>
To restore them to a standard look, add the 'link' class, making it appear as a <a href="#" class="link">normal link</a> once more.</p>
```

<!-- In cards -->

### In cards

Below is an example demonstrating how to use links in card.

```html
<div class="card max-w-sm">
  <div class="card-body">
    <h5 class="card-title mb-0">Card title</h5>
    <div class="text-base-content/50 mb-3">Card subtitle</div>
    <p class="mb-4">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <div class="card-actions">
      <a href="#" class="link link-primary link-hover">Card link</a>
      <a href="#" class="link link-primary link-animated">Another link</a>
    </div>
  </div>
</div>
```

<!-- In alerts -->

### In alerts

Below is an example demonstrating how to use links in alert.

```html
<div class="alert alert-soft" role="alert">
  Please read the support <a href="#" class="link">policy</a>.
</div>
```
