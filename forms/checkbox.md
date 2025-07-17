# Checkbox

The checkbox component allows users to select one or more options by ticking a square box, available in various styles, sizes, colors, and variants.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| checkbox | component | Component class for checkbox. |
| custom-option | component | For custom option container. |
| custom-soft-option | component | For custom option container with background. |
| label-text | part | Base class for title label text. |
| helper-text | part | Base class for helper label text. |
| checkbox-primary | color | Adds 'primary' color to checkbox. |
| checkbox-secondary | color | Adds 'secondary' color to checkbox. |
| checkbox-accent | color | Adds 'accent' color to checkbox. |
| checkbox-info | color | Adds 'info' color to checkbox. |
| checkbox-success | color | Adds 'success' color to checkbox. |
| checkbox-warning | color | Adds 'warning' color to checkbox. |
| checkbox-error | color | Adds 'error' color to checkbox. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| checkbox-xs | size | Checkbox with extra small size. |
| checkbox-sm | size | Checkbox with small size. |
| checkbox-md | size | Checkbox with medium(default) size. |
| checkbox-lg | size | Checkbox with large size. |
| checkbox-xl | size | Checkbox with extra large size. |


<!-------------------- Basic example -------------------->

## Basic example

<!--  Default  -->

### Default

Basic checkbox example.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox" id="defaultCheckbox1" />
  <label class="label-text text-base" for="defaultCheckbox1">Default</label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox" id="defaultCheckbox2" checked />
  <label class="label-text text-base" for="defaultCheckbox2">Checked</label>
</div>
```

<!--  Label and helper text  -->

### Label and helper text

Please use `label-text` for the label and `helper-text` for the text that appears at the bottom as helper text.

```html
<div class="flex gap-2">
  <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxLabel1" />
  <label class="label-text cursor-pointer flex flex-col" for="checkboxLabel1">
    <span class="text-base">Delete</span>
    <span>Notify me when this action happens.</span>
  </label>
</div>

<div class="flex gap-2">
  <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxLabel" checked />
  <label class="label-text cursor-pointer flex flex-col" for="checkboxLabel">
    <span class="text-base">Archive</span>
    <span>Notify me when this action happens.</span>
  </label>
</div>
```

<!-------------------- Color -------------------->

## Color

<!--  Semantic colors  -->

### Semantic colors

Apply a semantic color to the checkbox by using the `checkbox-{semantic-color}` modifier class together with the `checkbox` component class.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox" id="checkboxDefault" checked />
  <label class="label-text text-base" for="checkboxDefault"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-primary" id="checkboxPrimary" checked />
  <label class="label-text text-base" for="checkboxPrimary"> Primary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-secondary" id="checkboxSecondary" checked />
  <label class="label-text text-base " for="checkboxSecondary"> Secondary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-accent" id="checkboxAccent" checked />
  <label class="label-text text-base" for="checkboxAccent"> Accent </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-info" id="checkboxInfo" checked />
  <label class="label-text text-base" for="checkboxInfo"> Info </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-success" id="checkboxSuccess" checked />
  <label class="label-text text-base" for="checkboxSuccess"> Success </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-warning" id="checkboxWarning" checked />
  <label class="label-text text-base" for="checkboxWarning"> Warning </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-error" id="checkboxError" checked />
  <label class="label-text text-base" for="checkboxError"> Error </label>
</div>
```

<!--  Custom colors  -->

### Custom colors

To create custom checkboxes, you can use Tailwind CSS utilities like `bg-*`, `text-*` (for the tick), and `border-*` to style both the checked and unchecked states. With the `--input-color` value, you can easily modify the background and border color when the checkbox is checked. However, this will not affect the tick color, which by default uses the `neutral-content` text color. If you want to change the tick color, you will need to update the text color specifically for the checked state by using the `checked:text-*` utility.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checked:border-[#f0f] checked:bg-[#f0f] checked:text-[#fff]" id="checkboxCustomColor1" checked />
  <label class="label-text text-base" for="checkboxCustomColor1"> hex code </label>
</div>

<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checked:border-[green] checked:bg-[green] checked:text-white" id="checkboxCustomColor2" checked />
  <label class="label-text text-base" for="checkboxCustomColor2"> Named color </label>
</div>

<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checked:border-amber-400 checked:bg-amber-400 checked:text-amber-800" id="checkboxCustomColor5" checked/>
  <label class="label-text text-base" for="checkboxCustomColor5"> Tailwind utility colors </label>
</div>

<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox [--input-color:blue] checked:text-white" id="checkboxCustomColor5" checked/>
  <label class="label-text text-base" for="checkboxCustomColor5"> FlyonUI variable </label>
</div>
```

<!-------------------- Size -------------------->

## Size

<!--  Checkbox sizes  -->

### Checkbox sizes

Add responsive class `checkbox-{size}` where `{size} = xs|sm|md|lg|xl` for checkbox of different sizes.

```html
<div class="flex items-center">
  <input type="checkbox" class="checkbox checkbox-primary checkbox-xs" id="checkboxExtraSmall" checked />
  <label class="label-text text-xs" for="checkboxExtraSmall"> Extra small </label>
</div>
<div class="flex items-center gap-0.5">
  <input type="checkbox" class="checkbox checkbox-primary checkbox-sm" id="checkboxSmall" checked />
  <label class="label-text" for="checkboxSmall"> Small </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-primary" id="checkboxSizeDefault" checked />
  <label class="label-text text-base" for="checkboxSizeDefault"> Default </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="checkbox checkbox-primary checkbox-lg" id="checkboxLarge" checked />
  <label class="label-text text-lg" for="checkboxLarge"> Large </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="checkbox checkbox-primary checkbox-xl" id="checkboxExtraLarge" checked />
  <label class="label-text text-xl" for="checkboxExtraLarge"> Extra Large </label>
</div>
```

<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="flex gap-2">
  <input type="checkbox" class="checkbox checkbox-primary is-valid mt-2" id="checkboxStateSuccess" checked/>
  <label class="label-text cursor-pointer flex flex-col" for="checkboxStateSuccess">
    <span class="text-base">Delete</span>
    <span >Notify me when this action happens.</span>
  </label>
</div>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="flex gap-2">
  <input type="checkbox" class="checkbox checkbox-primary is-invalid mt-2" id="checkboxStateError" />
  <label class="label-text cursor-pointer flex flex-col" for="checkboxStateError">
    <span class="text-base">Delete</span>
    <span>Notify me when this action happens.</span>
  </label>
</div>
```

<!--------------------  Illustrations -------------------->

## Illustrations

<!--  Disabled  -->

### Disabled

Prevent user interaction with the checkbox by adding the `disabled` attribute to make it non-selectable.

```html
<input type="checkbox" class="checkbox" aria-label="disabled checkbox" checked disabled />
<input type="checkbox" class="checkbox" aria-label="disabled checkbox" disabled />
```

<!--  Indeterminate  -->

### Indeterminate

The `indeterminate` state can be configured using JavaScript. To gain further insight into this concept, you can explore more about it <a href="https://www.w3schools.com/jsref/prop_checkbox_indeterminate.asp" target="_blank" class="link link-primary">here</a>.

{{< code>}}

<div class="flex items-center gap-1">
  <input type="checkbox" class="checkbox checkbox-primary" id="check2" />
  <label class="label-text text-base" for="check2">Indeterminate</label>
</div>
<!-- js -->
<script>
  document.getElementById("check2").indeterminate = true
</script>
{{< /code >}}

<!--  Inline checkbox group  -->

### Inline checkbox group

A group of checkbox components.

```html
<div class="flex gap-4 overflow-x-auto">
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxInline1" />
    <label class="label-text text-base" for="checkboxInline1"> Vue </label>
  </div>
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxInline2" checked />
    <label class="label-text text-base" for="checkboxInline2"> Angular </label>
  </div>
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxInline3" />
    <label class="label-text text-base" for="checkboxInline3"> React </label>
  </div>
</div>
```

<!--  Vertical checkbox group  -->

### Vertical checkbox group

A vertical group of checkbox components.

```html
<div class="flex flex-col gap-2">
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxVertical1" />
    <label class="label-text text-base" for="checkboxVertical1"> Vue </label>
  </div>
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxVertical2" checked />
    <label class="label-text text-base" for="checkboxVertical2"> Angular </label>
  </div>
  <div class="flex items-center gap-2">
    <input type="checkbox" class="checkbox checkbox-primary" id="checkboxVertical3" />
    <label class="label-text text-base" for="checkboxVertical3"> React </label>
  </div>
</div>
```

<!--  Checkbox in dropdown  -->

### Checkbox in dropdown

Below example shows a checkbox in dropdown.

> **Info:** To learn more about dropdowns, refer to the [Dropdown](overlays/dropdown/) documentation.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-checkbox" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown checkbox
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60 space-y-0.5" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-checkbox">
    <div class="dropdown-item flex-col items-center gap-4 sm:flex-row sm:items-start">
      <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxDropdown1" checked />
      <label class="label-text cursor-pointer flex flex-col" for="checkboxDropdown1">
        <span class="font-semibold">Rename</span>
        <span class="text-base-content/50 text-base">Notify me when this action happens.</span>
      </label>
    </div>
    <div class="dropdown-item flex-col items-center gap-4 sm:flex-row sm:items-start">
      <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxDropdown2" />
      <label class="label-text cursor-pointer flex flex-col" for="checkboxDropdown2">
        <span class="font-semibold">Move</span>
        <span class="text-base-content/50 text-base">Notify me when this action happens.</span>
      </label>
    </div>
  </div>
</div>
```

<!--  Checkbox list group  -->

### Checkbox list group

This example can be used to show a list of checkbox buttons inside a grouped list.

```html
<h6 class="text-base-content mb-1 text-base">Select your favorite language:</h6>
<ul class="border-base-content/25 divide-base-content/25 rounded-box max-w-sm divide-y border *:cursor-pointer" >
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> C++ </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" checked />
      <span class="label-text text-base"> Ruby </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> Swift </span>
    </label>
  </li>
</ul>
```

<!--  Horizontal list group  -->

### Horizontal list group

Use this example to group up checkbox button components inside a list.

```html
<h6 class="text-base-content mb-1 text-base">Select your favorite language:</h6>
<ul
  class="border-base-content/25 divide-base-content/25 rounded-box flex w-full flex-col border *:w-full *:cursor-pointer max-sm:divide-y sm:flex-row sm:divide-x"
>
  <li class="w-full">
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> Python </span>
    </label>
  </li>
  <li class="w-full">
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" checked />
      <span class="label-text text-base"> JavaScript </span>
    </label>
  </li>
  <li class="w-full">
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> Java </span>
    </label>
  </li>
</ul>
```

<!-------------------- Custom Options -------------------->

## Custom options

<!--  Basic checkbox  -->

### Basic checkbox

The `custom-option` component is a flexible element with an associated label and background color, which can include text, icons, or images. It allows customization for layout, appearance, and interaction, providing various ways to enhance option designs.

```html
<div class="flex w-full flex-wrap items-start gap-3 sm:flex-nowrap">
  <label class="custom-option flex flex-row items-start gap-3 sm:w-1/2">
    <input type="checkbox" class="checkbox checkbox-primary mt-2" checked required />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Basic</span>
        <span class="text-base-content/50 text-base">Free</span>
      </span>
      <span class="text-base-content/80">Get 1 project with 1 teams members.</span>
    </span>
  </label>
  <label class="custom-option flex flex-row items-start gap-3 sm:w-1/2">
    <input type="checkbox" class="checkbox checkbox-primary mt-2" required />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Premium</span>
        <span class="text-base-content/50 text-base">$ 5.00</span>
      </span>
      <span class="text-base-content/80">Get 5 projects with 5 team members.</span>
    </span>
  </label>
</div>
```

<!--  Hidden checkbox button  -->

### Hidden checkbox button

Utilize the `hidden` utility class to conceal the checkbox button.

```html
<div class="flex w-full flex-wrap items-start gap-3 sm:flex-nowrap">
  <label class="custom-option flex flex-row items-start gap-4 sm:w-1/2">
    <input type="checkbox" class="checkbox hidden" checked />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Basic</span>
        <span class="text-base-content/50 text-base">Free</span>
      </span>
      <span class="text-base-content/80">Get 1 project with 1 teams members.</span>
    </span>
  </label>
  <label class="custom-option flex flex-row items-start gap-4 sm:w-1/2">
    <input type="checkbox" class="checkbox hidden" />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Premium</span>
        <span class="text-base-content/50 text-base">$ 5.00</span>
      </span>
      <span class="text-base-content/80">Get 5 projects with 5 team members.</span>
    </span>
  </label>
</div>
```

<!--  Basic label checkbox  -->

### Basic label checkbox

The `custom-soft-option` component is a flexible element that includes a background color, which becomes active when the option is selected. It can be used with any form of input, providing a visually distinct way to highlight the selected option.

```html
<div class="flex w-full flex-wrap items-start gap-3 sm:flex-nowrap">
  <label class="custom-soft-option flex flex-row items-start gap-3 sm:w-1/2">
    <input type="checkbox" class="checkbox checkbox-primary mt-2" checked />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Basic</span>
        <span class="text-base-content/50 text-base">Free</span>
      </span>
      <span class="text-base-content/80">Get 1 project with 1 teams members.</span>
    </span>
  </label>
  <label class="custom-soft-option flex flex-row items-start gap-3 sm:w-1/2">
    <input type="checkbox" class="checkbox checkbox-primary mt-2" />
    <span class="label-text w-full text-start">
      <span class="flex justify-between mb-1">
        <span class="text-base font-medium">Premium</span>
        <span class="text-base-content/50 text-base">$ 5.00</span>
      </span>
      <span class="text-base-content/80">Get 5 projects with 5 team members.</span>
    </span>
  </label>
</div>
```

<!--  Iconic custom checkbox  -->

### Iconic custom checkbox

Customize the checkbox styling using utility classes according to your preferences, as illustrated below.

```html
<div class="flex w-full items-start gap-3 flex-wrap sm:flex-nowrap">
  <label class="custom-option text-center flex sm:w-1/2 flex-col items-center gap-3">
    <span class="icon-[tabler--rocket] size-10"></span>
    <span class="flex flex-col label-text">
      <span class="text-base font-medium mb-1">Starter</span>
      <span class="text-base-content/80"> Cake sugar plum fruitcake I love sweet roll jelly-o</span>
    </span>
    <input type="checkbox" class="checkbox checkbox-primary" />
  </label>
  <label class="custom-option text-center flex sm:w-1/2 flex-col items-center gap-3">
    <span class="icon-[tabler--user] size-10"></span>
    <span class="flex flex-col label-text">
      <span class="text-base font-medium mb-1">Personal</span>
      <span class="text-base-content/80"> Cake sugar plum fruitcake I love sweet roll jelly-o.</span>
    </span>
    <input type="checkbox" class="checkbox checkbox-primary" checked />
  </label>
  <label class="custom-option text-center flex sm:w-1/2 flex-col items-center gap-3">
    <span class="icon-[tabler--crown] size-10"></span>
    <span class="flex flex-col label-text">
      <span class="text-base font-medium mb-1">Enterprise</span>
      <span class="text-base-content/80"> Cake sugar plum fruitcake I love sweet roll jelly-o.</span>
    </span>
    <input type="checkbox" class="checkbox checkbox-primary" />
  </label>
</div>
```

<!--  Image as checkbox  -->

### Image as checkbox

This example displays an image as a checkbox button.

```html
<div class="flex flex-nowrap items-start gap-3">
  <label class="custom-option relative p-0">
    <span class="w-full">
      <img src="https://cdn.flyonui.com/fy-assets/components/radio/image-6.png" class="bg-contain" alt="checkbox image" />
    </span>
    <input type="checkbox" class="checkbox checkbox-primary absolute end-0 top-0 m-3 hidden checked:block hover:block" />
  </label>
  <label class="custom-option relative p-0">
    <span class="w-full">
      <img src="https://cdn.flyonui.com/fy-assets/components/radio/image-3.png" class="bg-contain" alt="checkbox image" />
    </span>
    <input type="checkbox" class="checkbox checkbox-primary absolute end-0 top-0 m-3 hidden checked:block hover:block" checked />
  </label>
  <label class="custom-option relative p-0">
    <span class="w-full">
      <img src="https://cdn.flyonui.com/fy-assets/components/radio/image-5.png" class="bg-contain" alt="checkbox image" />
    </span>
    <input type="checkbox" class="checkbox checkbox-primary absolute end-0 top-0 m-3 hidden checked:block hover:block" />
  </label>
</div>
```
