# Pagination

Pagination is a set of controls, typically buttons or links, for navigating between multiple pages of content.

<!-- Class Table -->

| Class | Type | Description |
| --- | --- | --- |
| aria-[current='page']:{tw-utility-class} | modifier | Marks a pagination item as active by applying the corresponding utility class. |
| text-bg-{semantic-color} | modifier | Sets both text and background colors using the specified semantic color. |
| text-bg-soft-{semantic-color} | modifier | Applies a soft version of text and background colors using the selected semantic color. |
| text-border-{semantic-color} | modifier | Adds an outline styled with the chosen semantic color. |


> **Info:** To style pagination, we use the button component. For more information, see the [Button](components/button/) component documentation.

<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic pagination with the default style has been implemented. To denote the active state, we utilized `aria-[current='page']:{tw-utility-class}` for styling.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-text">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-text btn-square aria-[current='page']:text-bg-primary">1</button>
    <button type="button" class="btn btn-text btn-square aria-[current='page']:text-bg-primary" aria-current="page"> 2 </button>
    <button type="button" class="btn btn-text btn-square aria-[current='page']:text-bg-primary">3</button>
  </div>
  <button type="button" class="btn btn-text">Next</button>
</nav>
```

<!-------------------- Variants -------------------->

## Variants

<!-- Soft -->

### Soft

By applying the `btn-soft` modifier class, it will transform into a soft pagination type.
```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
```

<!-- Outline -->

### Outline

By applying the `btn-outline` modifier class, it will transform into a outline pagination type.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-outline">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-outline btn-square aria-[current='page']:text-border-primary aria-[current='page']:bg-primary/10" >1</button>
    <button type="button" class="btn btn-outline btn-square aria-[current='page']:text-border-primary aria-[current='page']:bg-primary/10" aria-current="page">2</button>
    <button type="button" class="btn btn-outline btn-square aria-[current='page']:text-border-primary aria-[current='page']:bg-primary/10" >3</button>
  </div>
  <button type="button" class="btn btn-outline">Next</button>
</nav>
```

<!-------------------- Shape -------------------->

## Shape

<!-- Default -->

### Default

Default shape example.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
```

<!-- Square -->

### Square

The `btn` class inherently includes the `rounded` utility, so by applying `rounded-none`, we can eliminate the rounded corners, creating square-shaped pagination.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft rounded-none">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary rounded-none">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary rounded-none" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary rounded-none">3</button>
  </div>
  <button type="button" class="btn btn-soft rounded-none">Next</button>
</nav>
```

<!-- Circle -->

### Circle

The `rounded-full` class rounds the "Previous" and "Next" buttons, while the `btn-circle` class creates circular pagination buttons.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft rounded-full">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-circle aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-circle aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-circle aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft rounded-full">Next</button>
</nav>
```

<!-------------------- Sizes -------------------->

## Sizes

<!-- Pagination sizes -->

### Pagination sizes

To create smaller or larger buttons, use the `btn-xs`, `btn-sm` and `btn-lg` responsive classes.

```html
<!--extra small button -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft btn-xs">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-xs btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-xs btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-xs btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft btn-xs">Next</button>
</nav>
<!-- small button -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft btn-sm">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-sm btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-sm btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-sm btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft btn-sm">Next</button>
</nav>
<!-- Default button -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
<!-- Large button -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft btn-lg">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-lg btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-lg btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-lg btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft btn-lg">Next</button>
</nav>
<!-- Extra Large button -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft btn-xl">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-xl btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-xl btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-xl btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft btn-xl">Next</button>
</nav>
```

<!-------------------- Alignment -------------------->

## Alignment

<!-- Pagination alignment -->

### Pagination alignment

To change the alignment of pagination components, use classes like `justify-center` to center them or `justify-end` to align them to the right.

```html
<!-- Default -->
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
<!-- justify-center -->
<nav class="flex items-center justify-center gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
<!-- justify-end -->
<nav class="flex items-center justify-end gap-x-1">
  <button type="button" class="btn btn-soft">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
```

<!-------------------- Responsive -------------------->

## Responsive

<!-- Text to icon -->

### Text to icon

On smaller screens, the text changes to an icon.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="hidden sm:block">Previous</span>
    <span class="icon-[tabler--chevron-left] rtl:rotate-180 block size-5 sm:hidden"></span>
  </button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="hidden sm:block">Next</span>
    <span class="icon-[tabler--chevron-right] rtl:rotate-180 block size-5 sm:hidden"></span>
  </button>
</nav>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Disabled -->

### Disabled

The previous button is disabled since it cannot go beyond page 1.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft btn-disabled">Previous</button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft">Next</button>
</nav>
```

<!-- Mini -->

### Mini

Mini size pagination.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-text btn-square" aria-label="Previous Button">
    <span class="icon-[tabler--chevron-left] size-5 rtl:rotate-180"></span>
  </button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-text btn-square pointer-events-none" aria-current="page">1</button>
    <span class="text-base-content/80 mx-3">of</span>
    <button type="button" class="btn btn-text btn-square pointer-events-none">3</button>
  </div>
  <button type="button" class="btn btn-text btn-square" aria-label="Next Button">
    <span class="icon-[tabler--chevron-right] size-5 rtl:rotate-180"></span>
  </button>
</nav>
```

<!-- Button group -->

### Button group

Group pagination uses the Join component.

> **Info:** For further details, refer to the [Join](forms/join/) component documentation.

```html
<nav class="join">
  <button type="button" class="btn btn-soft btn-square join-item" aria-label="Previous Button">
    <span class="icon-[tabler--chevron-left] size-5 rtl:rotate-180"></span>
  </button>
  <button type="button" class="btn btn-soft join-item btn-square aria-[current='page']:text-bg-soft-primary">1</button>
  <button type="button" class="btn btn-soft join-item btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
  <button type="button" class="btn btn-soft join-item btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  <button type="button" class="btn btn-soft btn-square join-item" aria-label="Next Button">
    <span class="icon-[tabler--chevron-right] size-5 rtl:rotate-180"></span>
  </button>
</nav>
```

<!-- With icon -->

### With icon

Utilize the provided code to display basic previous and next elements with icons.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="icon-[tabler--chevron-left] size-5 rtl:rotate-180"></span>
    <span class="hidden sm:inline">Previous</span>
  </button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
  </div>
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="hidden sm:inline">Next</span>
    <span class="icon-[tabler--chevron-right] size-5 rtl:rotate-180"></span>
  </button>
</nav>
```

<!-- Working with Tooltip -->

### Working with Tooltip

Pagination variant featuring tooltips.

```html
<nav class="flex items-center gap-x-1">
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="icon-[tabler--chevron-left] size-5 rtl:rotate-180 sm:hidden"></span>
    <span class="hidden sm:inline">Previous</span>
  </button>
  <div class="flex items-center gap-x-1">
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">1</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary" aria-current="page">2</button>
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">3</button>
    <!-- tooltip -->
    <div class="tooltip inline-block">
      <button type="button" class="tooltip-toggle tooltip-toggle btn btn-soft btn-square group" aria-label="More Pages">
        <span class="icon-[tabler--dots] size-5 group-hover:hidden"></span>
        <span class="icon-[tabler--chevrons-right] rtl:rotate-180 hidden size-5 shrink-0 group-hover:block"></span>
        <span class="tooltip-content tooltip-shown:opacity-100 tooltip-shown:visible" role="tooltip">
          <span class="tooltip-body">Next 7 pages</span>
        </span>
      </button>
    </div>
    <!-- tooltip end -->
    <button type="button" class="btn btn-soft btn-square aria-[current='page']:text-bg-soft-primary">10</button>
  </div>
  <button type="button" class="btn btn-soft max-sm:btn-square">
    <span class="hidden sm:inline">Next</span>
    <span class="icon-[tabler--chevron-right] size-5 rtl:rotate-180 sm:hidden"></span>
  </button>
</nav>
```
