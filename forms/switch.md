# Switch

Utilize the switch component to toggle between two states (true or false) with a single click. The component comes in multiple sizes, variants, and colors.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| switch | component | Component class for switch. |
| label-text | part | Base class for title label text. |
| helper-text | part | Base class for helper label text. |
| switch-outline | style | Component class outline switch. |
| switch-primary | color | Adds 'primary' color to switch. |
| switch-secondary | color | Adds 'secondary' color to switch. |
| switch-accent | color | Adds 'accent' color to switch. |
| switch-info | color | Adds 'info' color to switch. |
| switch-success | color | Adds 'success' color to switch. |
| switch-warning | color | Adds 'warning' color to switch. |
| switch-error | color | Adds 'error' color to switch. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| switch-xs | size | Switch with extra small size. |
| switch-sm | size | Switch with small size. |
| switch-md | size | Switch with medium size. |
| switch-lg | size | Switch with large size. |
| switch-xl | size | Switch with extra large size. |


<!--------------------  Basic example  -------------------->

## Basic example

<!--  Default  -->

### Default

Basic Switch example.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch" id="defaultSwitch1" />
  <label class="label-text text-base" for="defaultSwitch1"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch" id="defaultSwitch2" checked />
  <label class="label-text text-base" for="defaultSwitch2"> Checked </label>
</div>
```

<!--------------------  Type  -------------------->

## Type

<!--  Solid (Default)  -->

### Solid (Default)

For a switch style, apply the `switch` component class, whereas the default switch appearance is set to a solid color.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary" id="switchType1" />
  <label class="label-text text-base" for="switchType1"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary" id="switchType2" checked />
  <label class="label-text text-base" for="switchType2"> Checked </label>
</div>
```

<!--  Outline  -->

### Outline

To achieve an outline style for the switch, add component class `switch-outline` alongside `switch`.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-primary" id="switchType3" />
  <label class="label-text text-base" for="switchType3"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-primary" id="switchType4" checked />
  <label class="label-text text-base" for="switchType4"> Checked </label>
</div>
```

<!-------------------- Colors -------------------->

## Color

<!--  Semantic color  -->

### Semantic color

Example of semantic color in default and outline switch.

<!--  Default switch  -->

#### Default switch

Solid switch with semantic-color using `switch-{semantic-color}` modifier class with the component class `switch`.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch" id="switchDefault1" checked />
  <label class="label-text text-base" for="switchDefault1"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary" id="switchPrimary1" checked />
  <label class="label-text text-base" for="switchPrimary1"> Primary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-secondary" id="switchSecondary1" checked />
  <label class="label-text text-base" for="switchSecondary1"> Secondary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-accent" id="switchAccent1" checked />
  <label class="label-text text-base" for="switchAccent1"> Accent </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-info" id="switchInfo1" checked />
  <label class="label-text text-base" for="switchInfo1"> Info </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-success" id="switchSuccess1" checked />
  <label class="label-text text-base" for="switchSuccess1"> Success </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-warning" id="switchWarning1" checked />
  <label class="label-text text-base" for="switchWarning1"> Warning </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-error" id="switchError1" checked />
  <label class="label-text text-base" for="switchError1"> Error </label>
</div>
```

<!--  Outline switch  -->

#### Outline switch

Outline switch with semantic-color using `switch-{semantic-color}` modifier class with component classes `switch` & `switch-outline`.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline" id="switchDefault2" checked />
  <label class="label-text text-base" for="switchDefault2"> Default </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-primary" id="switchPrimary2" checked />
  <label class="label-text text-base" for="switchPrimary2"> Primary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-secondary" id="switchSecondary2" checked />
  <label class="label-text text-base" for="switchSecondary2"> Secondary </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-accent" id="switchAccent2" checked />
  <label class="label-text text-base" for="switchAccent2"> Accent </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-info" id="switchInfo2" checked />
  <label class="label-text text-base" for="switchInfo2"> Info </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-success" id="switchSuccess2" checked />
  <label class="label-text text-base" for="switchSuccess2"> Success </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-warning" id="switchWarning2" checked />
  <label class="label-text text-base" for="switchWarning2"> Warning </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-error" id="switchError2" checked />
  <label class="label-text text-base" for="switchError2"> Error </label>
</div>
```

<!--  Custom color  -->

### Custom color

Example of custom color in default and outline switch.

<!--  Default switch  -->

#### Default switch

Use `checked:text-*` to customize the ball color and `checked:bg-*` or `checked:border-*` to change the background and border when the switch is checked. Alternatively, you can use `checked:[--input-color:...]` to set both the background and border color when the switch is checked, simplifying customization. Supports hex, named colors, CSS variables, and Tailwind colors.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch checked:text-[#e4b0f8] checked:border-[#9b59b6] checked:bg-[#9b59b6]" id="switchCustomColor1" checked/>
  <label class="label-text text-base" for="switchCustomColor1"> Hex code </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch checked:text-[#8fff8f] checked:border-[green] checked:bg-[green]" id="switchCustomColor2" checked/>
  <label class="label-text text-base" for="switchCustomColor2"> Named color </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch checked:text-amber-100 checked:border-amber-600 checked:bg-amber-600" id="switchCustomColor4" checked/>
  <label class="label-text text-base" for="switchCustomColor4"> Tailwind utility colors </label>
</div>

<div class="flex items-center gap-1">
  <input type="checkbox" class="switch checked:text-blue-100 checked:[--input-color:blue]" id="switchCustomColor5" checked/>
  <label class="label-text text-base" for="switchCustomColor5"> FlyonUI variable </label>
</div>
```

<!--  Outline switch  -->

#### Outline switch

For `switch-outline`, use `--input-color` to set both the border and text color when the switch is checked. This eliminates the need to apply `checked:bg-*` and `checked:border-*` individually. You can still use `text-*` and `border-*` utilities to further customize the ball and border colors separately.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline checked:border-red-600 checked:text-blue-600" id="switchCustomColor6" checked />
  <label class="label-text text-base" for="switchCustomColor6"> Tailwind utility colors </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline checked:[--input-color:#9b59b6]" id="switchCustomColor7" checked />
  <label class="label-text text-base" for="switchCustomColor7"> With variable </label>
</div>
```

<!--------------------  Size  -------------------->

## Size

<!--  Solid switch  -->

### Solid switch

Add responsive class `switch-{size}` where `{size} = xs|sm|md|lg|xl` for switch of different sizes.

```html
<div class="flex items-center">
  <input type="checkbox" class="switch switch-xs switch-primary" id="switchExtraSmall1" checked />
  <label class="label-text text-xs" for="switchExtraSmall1"> Extra small switch </label>
</div>
<div class="flex items-center gap-0.5">
  <input type="checkbox" class="switch switch-sm switch-primary" id="switchSmall1" checked />
  <label class="label-text" for="switchSmall1"> Small switch </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary" id="switchSizeDefault1" checked />
  <label class="label-text text-base" for="switchSizeDefault1"> Default switch </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="switch switch-lg switch-primary" id="switchLarge1" checked />
  <label class="label-text text-lg" for="switchLarge1"> Large switch </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="switch switch-xl switch-primary" id="switchExtraLarge1" checked />
  <label class="label-text text-xl" for="switchExtraLarge1"> Extra large switch </label>
</div>
```

<!--  Outline switch  -->

### Outline switch

Add responsive class `switch-{size}` where `{size} = xs|sm|md|lg|xl` for switch of different sizes.

```html
<div class="flex items-center">
  <input type="checkbox" class="switch switch-outline switch-xs switch-primary" id="switchExtraSmall2" checked />
  <label class="label-text text-xs" for="switchExtraSmall2"> Extra small switch </label>
</div>
<div class="flex items-center gap-0.5">
  <input type="checkbox" class="switch switch-outline switch-sm switch-primary" id="switchSmall2" checked />
  <label class="label-text" for="switchSmall2"> Small switch </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-outline switch-primary" id="switchSizeDefault2" checked />
  <label class="label-text text-base" for="switchSizeDefault2"> Default switch </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="switch switch-outline switch-lg switch-primary" id="switchLarge2" checked />
  <label class="label-text text-lg" for="switchLarge2"> Large switch </label>
</div>
<div class="flex items-center gap-1.5">
  <input type="checkbox" class="switch switch-outline switch-xl switch-primary" id="switchExtraLarge2" checked />
  <label class="label-text text-xl" for="switchExtraLarge2"> Extra large switch </label>
</div>
```

<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="flex items-start gap-3">
  <input type="checkbox" class="switch switch-primary is-valid mt-2" id="switchStateSuccess1" checked /> 
  <label class="label-text cursor-pointer flex flex-col" for="switchStateSuccess1">
    <span class="text-base">Email Notifications</span>
    <span>Receive email notifications for updates</span>
  </label>
</div>
<div class="flex items-start gap-3">
  <input type="checkbox" class="switch switch-outline switch-primary is-valid mt-2" id="switchStateSuccess2" checked />
  <label class="label-text cursor-pointer flex flex-col" for="switchStateSuccess2">
    <span class="text-base">Dark Mode</span>
    <span>Enable dark mode for better readability</span>
  </label>
</div>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="flex items-start gap-3">
  <input type="checkbox" class="switch switch-primary is-invalid mt-2" id="switchStateError1" />
  <label class="label-text cursor-pointer flex flex-col" for="switchStateError1">
    <span class="text-base">Email Notifications</span>
    <span>Receive email notifications for updates</span>
  </label>
</div>
<div class="flex items-start gap-3">
  <input type="checkbox" class="switch switch-outline switch-primary is-invalid mt-2" id="switchStateError2" />
  <label class="label-text cursor-pointer flex flex-col" for="switchStateError2">
    <span class="text-base">Dark Mode</span>
    <span>Enable dark mode for better readability</span>
  </label>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!--  Switch with icon  -->

### Switch with icon

You can also add additional elements, such as icons.

```html
<!-- Default switch -->
<div class="space-x-3">
  <label class="relative inline-block">
    <input type="checkbox" class="switch switch-primary peer" aria-label="default switch with icon" />
    <span class="icon-[tabler--check] text-primary-content absolute start-1 top-1.5 hidden size-4 peer-checked:block" ></span>
    <span class="icon-[tabler--x] text-neutral-content absolute end-1 top-1.5  block size-4 peer-checked:hidden" ></span>
  </label>
  <label class="relative inline-block">
    <input type="checkbox" class="switch switch-primary peer" aria-label="default switch with icon" checked />
    <span class="icon-[tabler--check] text-primary-content absolute start-1 top-1.5 hidden size-4 peer-checked:block" ></span>
    <span class="icon-[tabler--x] text-neutral-content absolute end-1 top-1.5  block size-4 peer-checked:hidden" ></span>
  </label>
</div>

<!-- Outline switch -->

<div class="space-x-3">
  <label class="relative inline-block">
    <input type="checkbox" class="switch switch-primary switch-outline peer" aria-label="outline switch with icon" />
    <span class="icon-[tabler--check] text-primary absolute start-1 top-1.5 hidden size-4 peer-checked:block" ></span>
    <span class="icon-[tabler--x] text-neutral absolute end-1 top-1.5  block size-4 peer-checked:hidden" ></span>
  </label>
  <label class="relative inline-block">
    <input type="checkbox" class="switch switch-primary switch-outline peer" aria-label="outline switch with icon" checked />
    <span class="icon-[tabler--check] text-primary absolute start-1 top-1.5 hidden size-4 peer-checked:block" ></span>
    <span class="icon-[tabler--x] text-neutral absolute end-1 top-1.5  block size-4 peer-checked:hidden" ></span>
  </label>
</div>
```

<!--  Disabled  -->

### Disabled

Disabled switch
```html
<div class="space-x-3">
  <input type="checkbox" class="switch switch-primary" aria-label="disabled switch" disabled />
  <input type="checkbox" class="switch switch-primary" aria-label="disabled switch" checked disabled />
</div>
<div class="space-x-3">
  <input type="checkbox" class="switch switch-primary switch-outline" aria-label="outlined disabled switch" disabled />
  <input type="checkbox" class="switch switch-primary switch-outline" aria-label="outlined disabled switch" checked disabled />
</div>
```

<!--  Indeterminate  -->

### Indeterminate

The `indeterminate` state can be configured using JavaScript. To gain further insight into this concept, you can explore more about it <a href="https://www.w3schools.com/jsref/prop_checkbox_indeterminate.asp" target="_blank" class="link link-primary">here</a>.

```html
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary" id="switchSolid" />
  <label class="label-text text-base" for="switchSolid"> Solid switch </label>
</div>
<div class="flex items-center gap-1">
  <input type="checkbox" class="switch switch-primary switch-outline" id="switchOutline" />
  <label class="label-text text-base" for="switchOutline"> Outline switch </label>
</div>
 
<!-- js -->
<script>
  document.getElementById("switchSolid").indeterminate = true
  document.getElementById("switchOutline").indeterminate = true
</script>
```

<!--  Inline switch group  -->

### Inline switch group

A group of switch components in single line.

```html
<div class="flex gap-4 flex-col sm:flex-row">
  <div class="flex items-start gap-2">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchInline1" />
    <label class="label-text cursor-pointer flex flex-col" for="switchInline1">
      <span class="text-base">Email Notifications</span>
      <span>Receive email notifications for updates</span>
    </label>
  </div>
  <div class="flex items-start gap-2">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchInline2" checked />
    <label class="label-text cursor-pointer flex flex-col" for="switchInline2">
      <span class="text-base">Dark Mode</span>
      <span>Enable dark mode for better readability</span>
    </label>
  </div>
  <div class="flex items-start gap-2">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchInline3" />
    <label class="label-text cursor-pointer flex flex-col" for="switchInline3">
      <span class="text-base">Auto-Save</span>
      <span>Automatically save changes as you edit</span>
    </label>
  </div>
</div>
```

<!--  Vertical switch group  -->

### Vertical switch group

A vertical group of switch components.

```html
<div class="flex flex-col">
  <div class="flex items-start gap-4">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchVertical1" />
    <label class="label-text cursor-pointer flex flex-col" for="switchVertical1">
      <span class="text-base">Email Notifications</span>
      <span>Receive email notifications for updates</span>
    </label>
  </div>
  <div class="flex items-start gap-4">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchVertical2" checked />
    <label class="label-text cursor-pointer flex flex-col" for="switchVertical2">
      <span class="text-base">Dark Mode</span>
      <span>Enable dark mode for better readability</span>
    </label>
  </div>
  <div class="flex items-start gap-4">
    <input type="checkbox" class="switch switch-primary mt-2" id="switchVertical3" />
    <label class="label-text cursor-pointer flex flex-col" for="switchVertical3">
      <span class="text-base">Auto-Save</span>
      <span>Automatically save changes as you edit</span>
    </label>
  </div>
</div>
```

<!--  Switch in dropdown  -->

### Switch in dropdown

Here’s an example of a switch in dropdown.

> **Info:** To learn more about dropdowns, refer to the [Dropdown](overlays/dropdown/) documentation.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-checkbox" type="button" class="dropdown-switch btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown switch
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 min-w-60 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-checkbox">
    <div class="dropdown-item flex-col items-center gap-4 sm:flex-row sm:items-start">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown1" />
      <label class="label-text cursor-pointer flex flex-col" for="switchDropdown1">
        <span class="text-base">Email Notifications</span>
        <span>Receive email notifications for updates</span>
      </;>
    </div>
    <div class="dropdown-item flex-col items-center gap-4 sm:flex-row sm:items-start">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown2" checked />
      <label class="label-text cursor-pointer flex flex-col" for="switchDropdown2">
        <span class="text-base">Dark Mode</span>
        <span>Enable dark mode for better readability</span>
      </;>
    </div>
    <div class="dropdown-item flex-col items-center gap-4 sm:flex-row sm:items-start">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown3" />
      <label class="label-text cursor-pointer flex flex-col" for="switchDropdown3">
        <span class="text-base">Auto-Save</span>
        <span>Automatically save changes as you edit</span>
      </;>
    </div>
  </div>
</div>
```

<!--  Switch list group  -->

### Switch list group

This example can be used to show a list of switch inside a grouped list.

```html
<h6 class="text-base-content mb-1 text-base">Switch to your preferred languages:</h6>
<ul
  class="border-base-content/25 divide-base-content/25 rounded-box max-w-sm divide-y border *:cursor-pointer"
>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> JavaScript </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" checked />
      <span class="label-text text-base"> Python </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> Java </span>
    </label>
  </li>
</ul>
```

<!--  Horizontal list group  -->

### Horizontal list group

Use this example to group up switch components inside a list.

```html
<h6 class="text-base-content mb-1 text-base">Switch to your preferred languages:</h6>
<ul class="border-base-content/25 divide-base-content/25 rounded-box border flex w-full flex-col *:w-full *:cursor-pointer max-sm:divide-y sm:flex-row sm:divide-x" >
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> JavaScript </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" checked />
      <span class="label-text text-base"> Python </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> Java </span>
    </label>
  </li>
</ul>
```
