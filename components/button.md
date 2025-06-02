# Button

Browse and customize beautiful Tailwind CSS buttons in various styles and states, from active to disabled, allowing users to take actions or make choices.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| btn | component | Base class for the button component. |
| btn-soft | style | Soft colored button. |
| btn-outline | style | Transparent button with colored border. |
| btn-gradient | style | Gradient button |
| btn-primary | color | Button with 'primary' color. |
| btn-secondary | color | Button with 'secondary' color. |
| btn-accent | color | Button with 'accent' color. |
| btn-info | color | Button with 'info' color. |
| btn-success | color | Button with 'success' color. |
| btn-warning | color | Button with 'warning' color. |
| btn-error | color | Button with 'error' color. |
| btn-active | state | Force button to show active state. |
| btn-disabled | state | Force button to show disabled state. |
| btn-xs | size | Button with extra small size. |
| btn-sm | size | Button with small size. |
| btn-md | size | Button with medium(Default) size. |
| btn-lg | size | Button with large size. |
| btn-xl | size | Button with extra large size. |
| glass | modifier | Button with a glass effect. |
| btn-wide | modifier | Wide button (max-w-64). |
| btn-block | modifier | Full width button. |
| btn-circle | modifier | Circle button with a 1:1 ratio. |
| btn-square | modifier | Square button with a 1:1 ratio. |


<!-------------------- Variants -------------------->

## Variants

<!-- Solid buttons -->

### Solid buttons

The standard format for button is component class `btn`, accompanied by modifier class `btn-{semantic-color}`.

```html
<button class="btn">Default</button>
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-accent">Accent</button>
<button class="btn btn-info">Info</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-error">Error</button>
```

<!-- Soft buttons -->

### Soft buttons

Add modifier class `btn-soft` for soft colored buttons.

```html
<button class="btn btn-soft">Default</button>
<button class="btn btn-soft btn-primary">Primary</button>
<button class="btn btn-soft btn-secondary">Secondary</button>
<button class="btn btn-soft btn-accent">Accent</button>
<button class="btn btn-soft btn-info">Info</button>
<button class="btn btn-soft btn-success">Success</button>
<button class="btn btn-soft btn-warning">Warning</button>
<button class="btn btn-soft btn-error">Error</button>
```

<!-- Outline buttons -->

### Outline buttons

Add modifier class `btn-outline` for outline colored buttons.

```html
<button class="btn btn-outline">Default</button>
<button class="btn btn-outline btn-primary">Primary</button>
<button class="btn btn-outline btn-secondary">Secondary</button>
<button class="btn btn-outline btn-accent">Accent</button>
<button class="btn btn-outline btn-info">Info</button>
<button class="btn btn-outline btn-success">Success</button>
<button class="btn btn-outline btn-warning">Warning</button>
<button class="btn btn-outline btn-error">Error</button>
```


<!-- Text buttons -->

### Text buttons

Add modifier class `btn-text` for text colored buttons.

```html
<button class="btn btn-text">Default</button>
<button class="btn btn-text btn-primary">Primary</button>
<button class="btn btn-text btn-secondary">Secondary</button>
<button class="btn btn-text btn-accent">Accent</button>
<button class="btn btn-text btn-info">Info</button>
<button class="btn btn-text btn-success">Success</button>
<button class="btn btn-text btn-warning">Warning</button>
<button class="btn btn-text btn-error">Error</button>
```

<!-- Gradient buttons -->

### Gradient buttons

Add modifier class `btn-gradient` for gradient colored buttons.

```html
<button class="btn btn-gradient">Default</button>
<button class="btn btn-gradient btn-primary">Primary</button>
<button class="btn btn-gradient btn-secondary">Secondary</button>
<button class="btn btn-gradient btn-accent">Accent</button>
<button class="btn btn-gradient btn-info">Info</button>
<button class="btn btn-gradient btn-success">Success</button>
<button class="btn btn-gradient btn-warning">Warning</button>
<button class="btn btn-gradient btn-error">Error</button>
```

<!-- Wave effect button -->

### Wave effect button

Add modifier class `waves` for wave effect in buttons.

> **Info:** Refer [Wave Effect](third-party-plugins/wave-effect/) plugin for more details.

```html
<button class="btn btn-primary waves waves-light">Primary</button>
<button class="btn btn-soft btn-primary waves waves-primary">Primary</button>
<button class="btn btn-outline btn-primary waves waves-primary">Primary</button>
<button class="btn btn-text btn-primary waves waves-primary">Primary</button>
<button class="btn btn-gradient btn-primary waves waves-light">Primary</button>
```

<!-------------------- Shapes -------------------->

## Shapes

<!-- Pilled buttons -->

### Pilled buttons

Use the `rounded-full` utility class to make buttons circular. The default shape of the button but can be altered by using TailwindCSS <a href="https://tailwindcss.com/docs/border-radius" target="_blank" class="link link-primary">Border Radius</a> utility classes.

```html
<button class="btn btn-primary rounded-full">Primary</button>
<button class="btn btn-soft btn-primary rounded-full">Primary</button>
<button class="btn btn-outline btn-primary rounded-full">Primary</button>
<button class="btn btn-gradient btn-primary rounded-full">Primary</button>
```

<!-- Rounded buttons -->

### Rounded buttons

This is the default shape of button.

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-soft btn-primary">Primary</button>
<button class="btn btn-outline btn-primary">Primary</button>
<button class="btn btn-gradient btn-primary">Primary</button>
```

<!-------------------- State -------------------->

## States

<!-- States variants -->

### States variants

Use the `btn-active` class to force the button to show the active state and the `btn-disabled` class to force the button to show the disabled state.

Use state classes with any button variants.

```html
<button class="btn btn-primary">Default</button>
<button class="btn btn-primary btn-active">Active</button>
<button class="btn btn-primary btn-disabled">Disabled</button>
```

<!-------------------- Size -------------------->

## Size

<!-- Size variants -->

### Size variants

Add responsive class `btn-{size}` where `{size} = xs|sm|md|lg|xl` for button of different sizes.

> **Info:** For medium size button, use component class `btn`.

```html
<button class="btn btn-primary btn-xs">Tiny</button>
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary">Default</button>
<button class="btn btn-primary btn-lg">Large</button>
<button class="btn btn-primary btn-xl">Extra Large</button>
```

<!-- Wide button -->

### Wide button

To create a wide button, add the `btn-wide` class which provides additional horizontal padding.

```html
<button class="btn btn-primary btn-wide">Wide</button>
```

<!-- Block button -->

### Block button

To create a wide button, add the `btn-block` class which occupies the full width of the parent container.

```html
<button class="btn btn-primary btn-block">Block</button>
```

<!-- Responsive button -->

### Responsive button

This button will have different sizes on different browser viewpoints.

```html
<button class="btn btn-primary btn-sm md:btn-md lg:btn-lg">Responsive</button>
```

<!-------------------- Icons -------------------->

## Icon buttons

<!-- Icon at start/end -->

### Icon at start/end

Use any icons at start/end the button.

```html
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-primary"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span> Primary </button>
  <button class="btn btn-soft btn-primary"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span> Primary </button>
  <button class="btn btn-outline btn-primary"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span> Primary </button>
  <button class="btn btn-gradient btn-primary"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span> Primary </button>
</div>

<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-primary"> Primary <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
  <button class="btn btn-soft btn-primary"> Primary <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
  <button class="btn btn-outline btn-primary"> Primary <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
  <button class="btn btn-gradient btn-primary"> Primary <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
</div>
```

<!-- Icon only -->

### Icon only

Use `btn-square` or `btn-circle` to create circle/square button with a 1:1 ratio.

```html
<button class="btn btn-square btn-primary" aria-label="Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-square btn-soft btn-primary" aria-label="Soft Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-square btn-outline btn-primary" aria-label="Outline Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-square btn-gradient btn-primary" aria-label="Gradient Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-circle btn-primary" aria-label="Circle Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-circle btn-soft btn-primary" aria-label="Circle Soft Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-circle btn-outline btn-primary" aria-label="Circle Outline Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
<button class="btn btn-circle btn-gradient btn-primary" aria-label="Circle Gradient Icon Button"> <span class="icon-[tabler--star] size-4.5 shrink-0"></span></button>
```

<!-- Input tags -->

## Input tags

<!-- Buttons with input tags -->

### Buttons with input tags

You can use `btn` class on `<button>`, `<input>`, `<a>`, etc...

```html
<a role="button" class="btn">Link</a>
<button type="submit" class="btn">Button</button>
<input type="button" value="Input" class="btn" />
<input type="submit" value="Submit" class="btn" />
<input type="radio" aria-label="Radio" class="btn" />
<input type="checkbox" aria-label="Checkbox" class="btn" />
<input type="reset" value="Reset" class="btn" />
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Social buttons -->

### Social buttons

Use the following sample code to build custom Social, Payment, and other types of buttons. This example also demonstrates how to create a custom button using two variables: `--btn-color` and `--btn-fg`.

```html
<!-- Solid -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn [--btn-color:#1877F2] text-white" >
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span> Facebook
  </button>
  <button class="btn [--btn-color:#000] text-white" >
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span> Twitter
  </button>
  <button class="btn [--btn-color:#0a66c2] text-white" >
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span> LinkedIn
  </button>
  <button class="btn [--btn-color:#2b3137] text-white" >
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span> Github
  </button>
</div>

<!-- Soft -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-soft [--btn-color:#1877F2]">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span> Facebook
  </button>
  <button class="btn btn-soft [--btn-color:#000]">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span> Twitter
  </button>
  <button class="btn btn-soft [--btn-color:#0a66c2]">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span> LinkedIn
  </button>
  <button class="btn btn-soft [--btn-color:#2b3137]">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span> Github
  </button>
</div>

<!-- Outline -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-outline [--btn-color:#1877F2]">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span> Facebook
  </button>
  <button class="btn btn-outline [--btn-color:#000]">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span> Twitter
  </button>
  <button class="btn btn-outline [--btn-color:#0a66c2]">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span> LinkedIn
  </button>
  <button class="btn btn-outline [--btn-color:#2b3137]">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span> Github
  </button>
</div>

<!-- Text -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-text [--btn-color:#1877F2]">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span> Facebook
  </button>
  <button class="btn btn-text [--btn-color:#000]">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span> Twitter
  </button>
  <button class="btn btn-text [--btn-color:#0a66c2]">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span> LinkedIn
  </button>
  <button class="btn btn-text [--btn-color:#2b3137]">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span> Github
  </button>
</div>
```

Use `btn-square` or `btn-circle` to create circle/square buttons.

```html
<!-- Solid -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-square  [--btn-color:#1877F2] text-white" aria-label="Facebook Icon Button" >
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-square  [--btn-color:#000] text-white" aria-label="X Icon Button" >
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle  [--btn-color:#0a66c2] text-white" aria-label="Linkedin Icon Button" >
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle  [--btn-color:#2b3137] text-white" aria-label="Github Icon Button" >
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span>
  </button>
</div>

<!-- Soft -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-square btn-soft [--btn-color:#1877F2]" aria-label="Facebook Soft Icon Button">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-square btn-soft [--btn-color:#000]" aria-label="X Soft Icon Button">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-soft [--btn-color:#0a66c2]" aria-label="Linkedin Soft Icon Button">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-soft [--btn-color:#2b3137]" aria-label="Github Soft Icon Button">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span>
  </button>
</div>

<!-- Outline -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-square btn-outline [--btn-color:#1877F2]" aria-label="Facebook Outline Icon Button">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-square btn-outline [--btn-color:#000]" aria-label="X Outline Icon Button">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-outline [--btn-color:#0a66c2]" aria-label="Linkedin Outline Icon Button">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-outline [--btn-color:#2b3137]" aria-label="Github Outline Icon Button">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span>
  </button>
</div>

<!-- Text -->
<div class="flex w-full flex-wrap gap-2">
  <button class="btn btn-square btn-text [--btn-color:#1877F2]" aria-label="Facebook Outline Icon Button">
    <span class="icon-[tabler--brand-facebook] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-square btn-text [--btn-color:#1da1f2]" aria-label="X Outline Icon Button">
    <span class="icon-[tabler--brand-x] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-text [--btn-color:#0a66c2]" aria-label="Linkedin Outline Icon Button">
    <span class="icon-[tabler--brand-linkedin] size-4.5 shrink-0"></span>
  </button>
  <button class="btn btn-circle btn-text [--btn-color:#2b3137]" aria-label="Github Outline Icon Button">
    <span class="icon-[tabler--brand-github] size-4.5 shrink-0"></span>
  </button>
</div>
```

<!-- Loading buttons -->

### Loading buttons

Use loading component to add a loader to the button.

> **Info:** Refer [Loading Element](components/loading/) plugin for more details.

```html
<button class="btn btn-square btn-primary" aria-label="Loading Button">
<span class="loading loading-spinner"></span>
</button>

<button class="btn btn-primary">
  <span class="loading loading-spinner"></span>
  loading
</button>
```

<!-- Glass button -->

### Glass button

Use class `glass` to create a button with glass effect.

```html
<button class="btn glass">Glass button</button>
```


<!-- Dashed buttons -->

### Dashed buttons

You can achieve this style by combining the `border-dashed` utility class with the `btn-outline` modifier class.

```html
<button class="btn btn-outline border-dashed">Default</button>
<button class="btn btn-outline border-dashed btn-primary">Primary</button>
<button class="btn btn-outline border-dashed btn-secondary">Secondary</button>
<button class="btn btn-outline border-dashed btn-accent">Accent</button>
<button class="btn btn-outline border-dashed btn-info">Info</button>
<button class="btn btn-outline border-dashed btn-success">Success</button>
<button class="btn btn-outline border-dashed btn-warning">Warning</button>
<button class="btn btn-outline border-dashed btn-error">Error</button>
```

<!-- Button group -->

### Button group

Group a series of buttons together on a single line or stack them in a vertical/horizontal column

{{< callout "info" false >}}
Refer the [Join](forms/join/) component documentation for creating a group of buttons.
{{< /callout >}}

```html
<div class="join">
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
</div>
```
