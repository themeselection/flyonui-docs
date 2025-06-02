# Join (Group Items)

Join acts as a container for grouping items like buttons and inputs, applying border radius to the first and last items for horizontal or vertical lists.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| join | component | Container for grouping multiple items |
| join-item | part | Item inside join. Can be a button, input, etc. |
| join-vertical | direction | Show items vertically |
| join-horizontal | direction | Show items vertically |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic join elements example.

```html
<div class="join">
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
</div>
```

<!-- Icons -->

### Icons

Basic join elements example using icons.

```html
<div class="join">
  <button class="btn btn-soft btn-primary btn-square join-item" aria-label="join"><span class="icon-[tabler--star]"></span></button>
  <button class="btn btn-soft btn-primary btn-square join-item" aria-label="join"><span class="icon-[tabler--star]"></span></button>
  <button class="btn btn-soft btn-primary btn-square join-item" aria-label="join"><span class="icon-[tabler--star]"></span></button>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Vertical -->

### Vertical

Group items vertically.

```html
<div class="join join-vertical drop-shadow-sm">
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
</div>
```

<!-- Responsive -->

### Responsive

it's vertical on small screen and horizontal on large screen.

```html
<div class="join max-sm:join-vertical">
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
  <button class="btn btn-soft btn-primary join-item">Button</button>
</div>
```

<!-- Multiple elements -->

### Multiple elements

Basic join example illustrating the integration of multiple elements.

```html
<div class="join max-w-sm">
  <input class="input join-item" placeholder="Search" />
  <select class="select join-item" aria-label="select">
    <option disabled selected>Filter</option>
    <option>Sci-fi</option>
    <option>Drama</option>
    <option>Action</option>
  </select>
  <button class="btn btn-soft btn-primary join-item">Search</button>
</div>
```

<!-- Pill shape -->

### Pill shape

The default shape of the join can be altered by using TailwindCSS <a href="https://tailwindcss.com/docs/border-radius" target="_blank" class="link link-primary">Border Radius</a> utility classes.

```html
<div class="join">
  <input class="input join-item rounded-s-full" placeholder="Email" />
  <button class="btn btn-soft btn-primary join-item rounded-e-full">Subscribe</button>
</div>
```

<!-- Dropdown with input -->

### Dropdown with input

You can also join `input` and `dropdown`.

> **Info:** To learn more about dropdowns, refer to the [Dropdown](overlays/dropdown/) documentation.

```html
<div class="join">
  <input class="input join-item shrink" placeholder="Email" />
  <div class="dropdown relative inline-flex max-sm:[--placement:bottom-end]">
    <button id="dropdown-input" type="button" class="dropdown-toggle btn btn-soft btn-primary join-item" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      <span class="hidden sm:block">Dropdown</span>
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-input">
      <li><a class="dropdown-item" href="#">Subscribe</a></li>
      <li><a class="dropdown-item" href="#">Verify</a></li>
    </ul>
  </div>
</div>
```
