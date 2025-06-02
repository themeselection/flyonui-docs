# Theme Controller

If a checkbox or radio input with the theme-controller class is present on the page, the page's theme will be set to the value of that input.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| theme-controller | component | For a checkbox or radio button input intended to toggle the page theme. |


The Theme Controller changes the theme using only CSS. You can use JavaScript to save the input state to the server or localStorage if you want it to persist across page refreshes.

<!-------------------- Basic example -------------------->

## Basic example

<!-- Checkbox -->

### Checkbox

Use the `theme-controller` component class with a checkbox input to create a theme switcher that toggles between the default theme and the theme specified in the value.

```html
<input type="checkbox" value="dark" class="checkbox theme-controller" />
```

<!-- Switch -->

### Switch

Create a theme controller using a switch based on the example provided below.

```html
<input type="checkbox" value="dark" class="switch theme-controller" />
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Using swap -->

### Using swap

The example below shows how to implement a theme controller using a switch component.

```html
<label class="swap swap-rotate">
  <input type="checkbox" value="dark" class="theme-controller" />
  <span class="swap-off icon-[tabler--sun] size-7"></span>
  <span class="swap-on icon-[tabler--moon] size-7"></span>
</label>
```

<!-- Using switch with text -->

### Using switch with text

The example below illustrates how to create a theme controller using a switch combined with text.

```html
<label class="flex cursor-pointer gap-2">
  <span class="label-text">Light</span>
  <input type="checkbox" value="dark" class="switch theme-controller" />
  <span class="label-text">Dark</span>
</label>
```

<!-- Using switch with icons inside -->

### Using switch with icons inside

The example provided shows how to build a theme controller using a switch that features icons.

```html
<label class="relative inline-block">
    <input type="checkbox" class="switch switch-primary theme-controller peer" aria-label="default switch with icon" checked />
    <span class="icon-[tabler--sun] text-primary-content absolute start-1 top-1.5 hidden size-4 peer-checked:block" ></span>
    <span class="icon-[tabler--moon] text-neutral-content absolute end-1 top-1.5  block size-4 peer-checked:hidden" ></span>
  </label>
```

<!-- Using switch with custom colors -->

### Using a switch with custom colors

The example below shows how to build a theme controller using a switch with personalized colors.

```html
<input type="checkbox" value="dark" class="switch theme-controller checked:text-[#e4b0f8] checked:border-[#9b59b6] checked:bg-[#9b59b6]" />
```

<!-- Using radio input -->

### Using a radio input

Create a theme controller using a radio input based on the example below.

```html
<div class="flex flex-col gap-1">
  <div>
    <div class="flex items-center justify-between gap-4">
      <label class="label-text" for="defaultTheme">Default</label>
      <input type="radio" name="theme-radios" class="radio theme-controller" id="defaultTheme" value="default" checked />
    </div>
  </div>
  <div>
    <div class="flex items-center justify-between gap-4">
      <label class="label-text" for="corporateTheme">Corporate</label>
      <input type="radio" name="theme-radios" class="radio theme-controller" id="corporateTheme" value="corporate" />
    </div>
  </div>
  <div>
    <div class="flex items-center justify-between gap-4">
      <label class="label-text" for="gourmentTheme">Gourmet</label>
      <input type="radio" name="theme-radios" class="radio theme-controller" id="gourmentTheme" value="gourmet" />
    </div>
  </div>
</div>
```

<!--  Using radio button -->

### Using a radio button

The example below shows how to create a theme controller using a radio button.

```html
<div class="join drop-shadow join-vertical">
  <input type="radio" name="theme-buttons" class="btn btn-secondary theme-controller join-item" aria-label="Default" value="default" checked />
  <input type="radio" name="theme-buttons" class="btn btn-secondary theme-controller join-item" aria-label="Corporate" value="corporate" />
  <input type="radio" name="theme-buttons" class="btn btn-secondary theme-controller join-item" aria-label="Gourmet" value="gourmet" />
</div>
```

<!-- Using a dropdown -->

### Using a dropdown

Here's a ready-to-use example of a theme controller utilizing a dropdown menu.

> **Info:** For more information about dropdowns, refer to the [Dropdown](overlays/dropdown/) documentation.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-default" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown" >
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default" >
    <li>
      <input type="radio" name="theme-dropdown" class="theme-controller btn btn-text w-full justify-start" aria-label="Default" value="default" checked />
    </li>
    <li>
      <input type="radio" name="theme-dropdown" class="theme-controller btn btn-text w-full justify-start" aria-label="Corporate" value="corporate" />
    </li>
    <li>
      <input type="radio" name="theme-dropdown" class="theme-controller btn btn-text w-full justify-start" aria-label="Gourmet" value="gourmet" />
    </li>
  </ul>
</div>
```

<!-------------------- JavaScript Behavior -------------------->
## JavaScript Behavior

<!-- Saving Theme Preferences in Local Storage -->

### Saving Theme Preferences in Local Storage

> **Info:** The <a href="https://github.com/saadeghi/theme-change" target="_blank" class="link link-primary font-medium">theme-change</a> plugin by daisyUI is a powerful tool for implementing dynamic theme switching in your projects. It allows users to select, toggle, or customize themes while seamlessly saving their preferences in local storage for a consistent user experience.  

<!-- Setup -->
### Setup

Below are the comprehensively outlined steps you can follow to seamlessly integrate <a href="https://github.com/saadeghi/theme-change" target="_blank" class="link link-primary font-semibold">theme-change</a> into your project for efficient theme switching functionality with storing in local storage.

<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full mb-12 ps-0">
  <!-- Installation -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        1
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Step 1: Install theme-change</div>
      <p>
        Install
        <code>theme-change</code>
        via npm.
      </p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}npm i theme-change --save{{< /code-highlight >}}
    </div>
    <hr class="rounded-none border-transparent !w-0.5" />
  </li>

  <!-- Include it in javascript file -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        2
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Step 2: Include it in javascript file.</div>
      <p>
        To integrate theme-change, add the following
        <code>code</code>
        in your
        <code>javascript</code>
        file.
      </p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="js" >}}import { themeChange } from 'theme-change'
themeChange(){{< /code-highlight >}}
      <div class="text-base-content my-3 font-semibold">You can also use a CDN link.</div>
      <p>Include the following <code>&lt;script&gt;</code> tag near the end of your <code>&lt;/body&gt;</code> section:</p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="html" >}}<script src="https://cdn.jsdelivr.net/npm/theme-change@2.0.2/index.js"></script>{{< /code-highlight >}}
    </div>
    <hr class="rounded-none border-transparent !w-0.5" />
  </li>

  <!-- Basic use case of theme-change -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        3
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Step 3: Basic use case of theme-change.</div>
      <p>
        The below example showcase the toggle functionality using the switch component.
      </p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="html" >}}<input type="checkbox" data-toggle-theme="luxury" class="switch" />{{< /code-highlight >}}
    </div>
  </li>
</ul>

The `theme-change` plugin offers three primary attributes to manage themes dynamically:

1. `data-set-theme="luxury"`  
   Use this attribute to set the theme directly for components such as buttons, radio buttons, and dropdowns. The theme is applied upon user interaction (e.g., clicking a button).  

2. `data-choose-theme`  
   This attribute is designed for `select` components. It dynamically applies the theme based on the selected option from a dropdown menu.  

3. `data-toggle-theme="soft"`  
   Ideal for toggle components like checkboxes and switches. This attribute allows users to switch between themes interactively by toggling the element.  

It also provides the `data-act-class="ACTIVECLASS"` attribute, which applies the specified `ACTIVECLASS` to the element when it is clicked or toggled.

For a live demonstration and detailed example of using FlyonUI with the `theme-change` plugin, check out this <a href="https://stackblitz.com/edit/flyonui-theme-switcher-4dfjut-uyqsr9?file=index.html" target="_blank" class="link link-primary font-medium">StackBlitz example</a>.
