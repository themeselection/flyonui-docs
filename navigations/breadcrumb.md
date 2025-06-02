# Breadcrumb

A breadcrumb is a secondary navigation scheme that reveals the user's location in a website or web application.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| breadcrumbs | component | Base class for breadcrumb component. |
| breadcrumbs-separator | part | Used to separate icons or text within breadcrumbs. |


<!-------------------- Variants -------------------->

## Variants

<!-- With chevrons -->

### With chevrons

Utilize the component class `breadcrumbs` to generate a breadcrumb component. By integrating a chevron icon within the `breadcrumbs-separator` component class, you can create breadcrumbs with chevrons as separators.

```html
<div class="breadcrumbs">
  <ul>
    <li>
      <a href="#">Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li>
      <a href="#">Components</a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li aria-current="page">Breadcrumb</li>
  </ul>
</div>
```

<!-- With slashes -->

### With slashes

Using `/` in the `breadcrumbs-separator` class creates breadcrumbs with chevron separators, while the `rtl:` Tailwind modifier ensures smooth RTL mode operation.

For more information, check out the TailwindCSS <a href="https://tailwindcss.com/docs/hover-focus-and-other-states#rtl-support" target="_blank" class="link link-primary">RTL support</a> documentation.

```html
<div class="breadcrumbs">
  <ul>
    <li>
      <a href="#">Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <a href="#">Components</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li aria-current="page">Breadcrumb</li>
  </ul>
</div>
```

<!-- With icons -->

### With icons

Add icons in `<a>` tag to create breadcrumbs with icons.

```html
<div class="breadcrumbs">
  <ol>
    <li>
      <a href="#"> <span class="icon-[tabler--star-filled] size-5"></span>Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li>
      <a href="#"> <span class="icon-[tabler--star-filled] size-5"></span>Components</a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li aria-current="page">
      <span class="icon-[tabler--star-filled] me-1 size-5"></span>
      Breadcrumb
    </li>
  </ol>
</div>
```

<!-------------------- Functionality -------------------->

## Functionality

<!-- Multiple pages -->

### Multiple pages

Use the below given example to show breadcrumbs with multiple pages.

```html
<div class="breadcrumbs">
  <ol>
    <li>
      <a href="#"> <span class="icon-[tabler--folder] size-5"></span>Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li>
      <a href="#" aria-label="More Pages"><span class="icon-[tabler--dots]"></span></a>
    </li>
    <li class="breadcrumbs-separator rtl:rotate-180"><span class="icon-[tabler--chevron-right]"></span></li>
    <li aria-current="page">
      <span class="icon-[tabler--file] me-1 size-5"></span>
      Breadcrumb
    </li>
  </ol>
</div>
```

<!-- With dropdown -->

### With dropdown

Use dropdowns with breadcrumbs for versatile navigation.

> **Info:** To learn more about dropdowns, refer to the [Dropdown](overlays/dropdown/) documentation.

```html
<div class="breadcrumbs">
  <ol>
    <li>
      <a href="#">Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <div class="dropdown relative inline-flex">
        <button id="dropdown-default" type="button" class="dropdown-toggle btn btn-text font-normal" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
          Components
          <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
        </button>
        <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-10" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default">
          <li><a class="dropdown-item" href="#">Overlay</a></li>
          <li><a class="dropdown-item" href="#">Navigation</a></li>
          <li><a class="dropdown-item" href="#">Collapse</a></li>
          <li><a class="dropdown-item" href="#">Form</a></li>
        </ul>
      </div>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li aria-current="page">
      <div class="dropdown relative inline-flex">
        <button id="dropdown-default" type="button" class="dropdown-toggle btn btn-text btn-secondary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
          Component
          <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
        </button>
        <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-10" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default">
          <li><a class="dropdown-item" href="#">Modal</a></li>
          <li><a class="dropdown-item" href="#">Breadcrumb</a></li>
          <li><a class="dropdown-item" href="#">Accordion</a></li>
          <li><a class="dropdown-item" href="#">Input</a></li>
        </ul>
      </div>
    </li>
  </ol>
</div>
```

<!-- With max-width -->

### With max-width

Apply the responsive utility class `max-w-xs` to the breadcrumb, enabling a fixed width that allows horizontal scrolling while occupying less space.

```html
<div class="breadcrumbs h-fit max-w-xs">
  <ul>
    <li>
      <a href="#"> <span class="icon-[tabler--folder] size-5"></span>Home</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <a href="#"> <span class="icon-[tabler--folder] size-5"></span>App</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <a href="#"> <span class="icon-[tabler--folder] size-5"></span>Components</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <a href="#"> <span class="icon-[tabler--folder] size-5"></span>Navigation</a>
    </li>
    <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
    <li>
      <span class="icon-[tabler--file] me-1 size-5"></span>
      Breadcrumb
    </li>
  </ul>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- With background -->

### With background

Use the below given example for breadcrumb with background.

```html
<div class="w-full rounded-lg border px-4 py-2">
  <div class="breadcrumbs">
    <ul>
      <li>
        <a href="#">Home</a>
      </li>
      <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
      <li>
        <a href="#">Components</a>
      </li>
      <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
      <li aria-current="page">
        <span class="bg-primary/20 !text-primary rounded-xs px-1.5 py-0.5">Breadcrumb</span>
      </li>
    </ul>
  </div>
</div>
```

<!-- Bordered breadcrumb -->

### Bordered breadcrumb

Use the below given example for breadcrumb with border.

```html
<div class="border-base-content/25 w-full rounded-lg border px-4 py-2">
  <div class="breadcrumbs">
    <ul>
      <li>
        <a href="#">Home</a>
      </li>
      <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
      <li>
        <a href="#">Components</a>
      </li>
      <li class="breadcrumbs-separator rtl:-rotate-[40deg]">/</li>
      <li aria-current="page">Breadcrumb</li>
    </ul>
  </div>
</div>
```
