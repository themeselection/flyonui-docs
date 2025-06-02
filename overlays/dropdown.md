# Dropdown

The Dropdown neatly displays Dropdown or content using a JavaScript plugin, offering a compact interface for easy navigation and space-saving.

> **Info:** Dropdown components are adopted from <a href="https://preline.co/docs/dropdown.html" target="_blank" class="link link-primary font-semibold">Preline UI</a> components using <a href="https://preline.co/plugins.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

> We harnessed <a href="https://floating-ui.com/" class="link link-primary font-semibold" target="blank">FloatingUI</a> to supercharge our dropdown experience.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| dropdown | component | Container for the dropdown. |
| dropdown-toggle | part | Toggle button for the dropdown. |
| dropdown-menu | part | Container for the dropdown menu. |
| dropdown-title | part | Adds a title to the dropdown. |
| dropdown-header | part | Adds a header to the dropdown. |
| dropdown-footer | part | Adds a footer to the dropdown. |
| dropdown-toggle-wrapper | part | A wrapper for a Dropdown toggle, this is useful when some other element is placed in the Dropdown toggle. For example. if you want to place a "+" button inside an existing Dropdown toggle button that opens a modal. |
| dropdown-item | part | Styles applied to individual dropdown items. |
| dropdown-open:{tw-utility-class} | variant | Modifies tailwind classes when the dropdown menu is open. |
| dropdown-close | modifier | Dropdown close element (can be multiple). |
| dropdown-active | state | Applies active styling to dropdown items. |
| dropdown-disabled | state | Applies disabled styling to dropdown items. |



<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic dropdown example.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-default" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-------------------- Menu Content -------------------->

## Menu content

<!-- Dropdown header -->

### Dropdown header

Use `dropdown-header` class to display extra information separately from the menu items in the dropdown.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-header" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown header
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-header">
    <li class="dropdown-header gap-2">
      <div class="avatar">
        <div class="w-10 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
        </div>
      </div>
      <div>
        <h6 class="text-base-content text-base font-semibold">John Doe</h6>
        <small class="text-base-content/50 text-sm font-normal">jhon@doe.com</small>
      </div>
    </li>
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Dropdown footer -->

### Dropdown footer

Use the `dropdown-footer` class to present additional information distinct from the dropdown menu items, at the
bottom.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-footer" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown footer
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-footer">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
    <li class="dropdown-footer gap-2">
      <button class="btn btn-error btn-soft btn-block">Sign out</button>
    </li>
  </ul>
</div>
```

<!-- Dropdown title -->

### Dropdown title

Use `dropdown-title` class to present titile for the dropdown content.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-title" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown title
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-title">
    <li class="dropdown-title">Settings</li>
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
    <hr class="border-base-content/25 my-2 -mx-2" />
    <li class="dropdown-title">Contact</li>
    <li><a class="dropdown-item" href="#">Contact support</a></li>
  </ul>
</div>
```

<!-- Dropdown form -->

### Dropdown form

Using form within a dropdown menu.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-form" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown form
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 min-w-70 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-form">
    <form class="p-4">
      <div class="mb-4">
        <label class="label-text" for="username"> Username </label>
        <input type="text" placeholder="Johndoe" class="input" id="username" />
      </div>
      <div class="mb-4">
        <label class="label-text" for="password"> Password </label>
        <input type="password" placeholder="············" class="input" id="password" autocomplete="password" />
      </div>
      <button type="submit" class="btn btn-primary btn-block">Sign in</button>
    </form>
  </div>
</div>
```

<!-- Dropdown radio -->

### Dropdown radio

Put radio inside `dropdown-item`. Make the dropdown item appear with radio.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-transportation" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown radio
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-transportation">
    <div class="dropdown-item gap-4">
      <input id="dropdown-radio-car-2" name="dropdown-item-radio" type="radio" class="radio radio-primary" checked/>
      <label for="dropdown-radio-car-2" class="label-text text-base-content block text-sm font-semibold">Car </label>
    </div>
    <div class="dropdown-item gap-4">
      <input id="dropdown-radio-bicycle-2" name="dropdown-item-radio" type="radio" class="radio radio-primary" />
      <label for="dropdown-radio-bicycle-2" class="label-text text-base-content text-sm font-semibold"> Bicycle </label>
    </div>
  </div>
</div>
```

<!-- Dropdown checkbox -->

### Dropdown checkbox

Put checkbox inside `dropdown-item`. Make the dropdown item appear with checkbox.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-checkbox" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown checkbox
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-checkbox">
    <div class="dropdown-item items-start gap-4 max-sm:px-2">
      <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxDropdown-1" checked />
      <label class="label-text flex flex-col items-start" for="checkboxDropdown-1">
        <span class="font-semibold">Mark as important</span>
        <span class="text-base-content/50">Notify me when this action happens.</span>
      </label>
    </div>
    <div class="dropdown-item items-start gap-4 max-sm:px-2">
      <input type="checkbox" class="checkbox checkbox-primary mt-2" id="checkboxDropdown-2" />
      <label class="label-text flex flex-col items-start" for="checkboxDropdown-2">
        <span class="font-semibold">Share with team</span>
        <span class="text-base-content/50">Notify me when this action happens.</span>
      </label>
    </div>
  </div>
</div>
```

<!-- Dropdown with switch -->

### Dropdown with switch

Put switch inside `dropdown-item`. Make the dropdown item appear with switch.

```html
<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-checkbox" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown switch
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 min-w-60 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-checkbox">
    <div class="dropdown-item items-start gap-4">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown-1" checked />
      <label class="label-text flex flex-col items-start" for="switchDropdown-1">
        <span class="text-base">Notifications</span>
        <span>Receive push notifications</span>
      </label>
    </div>
    <div class="dropdown-item items-start gap-4">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown-2" />
      <label class="label-text flex flex-col items-start" for="switchDropdown-2">
        <span class="text-base">Location Services</span>
        <span>Allow access to your location</span>
      </label>
    </div>
    <div class="dropdown-item items-start gap-4">
      <input type="checkbox" class="switch switch-primary mt-2" id="switchDropdown-2" checked />
      <label class="label-text flex flex-col items-start" for="switchDropdown-3">
        <span class="text-base">Dark Theme</span>
        <span>Enable dark theme for the app</span>
      </label>
    </div>
  </div>
</div>
```

<!-- Dropdown within dropdown -->

### Nested dropdowns

Create nested dropdowns by adding a dropdown within a dropdown.

```html
<div class="dropdown relative inline-flex">
  <button id="nested-dropdown" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="nested-dropdown">
    <li><a class="dropdown-item" href="#">Send My Profile</a></li>
    <li><a class="dropdown-item" href="#">View Settings</a></li>
    <li class="dropdown relative [--offset:15] [--placement:right-start]">
      <button id="nested-dropdown-2" class="dropdown-toggle dropdown-item justify-between"  aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
        More Options
        <span class="icon-[tabler--chevron-right] size-4 rtl:rotate-180"></span>
      </button>
      <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="nested-dropdown-2">
        <li><a class="dropdown-item" href="#">Download Documents</a></li>
        <li><a class="dropdown-item" href="#">Manage FAQs</a></li>
      </ul>
    </li>
    <li><a class="dropdown-item" href="#">Logout</a></li>
  </ul>
</div>
```

<!-------------------- Custom Trigger -------------------->

## Custom trigger

<!-- Menu icon -->

### Menu icon

Use the menu icon trigger element on components such as cards as an alternative element to the button.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-menu-icon" type="button" class="dropdown-toggle btn btn-square btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    <span class="icon-[tabler--dots-vertical] size-6"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-menu-icon">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Split dropdown -->

### Split dropdown

Demonstration of a split dropdown.

```html
<div class="join">
  <button type="button" class="btn btn-outline btn-primary join-item">Dropdown</button>
  <div class="dropdown relative inline-flex">
    <button id="dropdown-split" type="button" class="dropdown-toggle btn btn-square btn-primary join-item" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-split">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>
</div>
```

<!-- Trigger with avatar -->

### Trigger with avatar

Dropdown with avatar.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-avatar" type="button" class="dropdown-toggle btn btn-outline btn-primary flex items-center gap-2 rounded-full" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    <div class="avatar">
      <div class="size-6 rounded-full">
        <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Avatar" />
      </div>
    </div>
    John Doe
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-avatar">
    <li class="dropdown-header gap-3">
      <div class="avatar">
        <div class="w-10 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Avatar" />
        </div>
      </div>
      <div>
        <h6 class="text-base-content text-base font-semibold">John Doe</h6>
        <small class="text-base-content/50 text-sm font-normal">jhon@doe.com</small>
      </div>
    </li>
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-------------------- Animations -------------------->

## Animations

<!-- Slide up animation -->

### Slide up animation

The basic dropdown menu featuring a slide-up animation.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-Slide" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu transition-[opacity,margin] duration-300 dropdown-open:opacity-100 hidden min-w-60 mt-2" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-Slide">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Transform animation -->

### Transform animation

Use `dropdown-open:{tw-utility-class}` modifier to introduce animation to your dropdown menu. The following example demonstrates a scaling animation.

> **Info:** To create a slide-up animation effect, we use `mt-2`. However, if you're crafting your own animation, add `mt-0` to avoid a jumpy effect upon closing.

```html
<div class="w-full">
  <div class="dropdown relative inline-flex  [--strategy:absolute]">
    <button id="dropdown-transform" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Dropdown
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 dropdown-open:ease-in dropdown-open:scale-100 mt-0 hidden min-w-60 origin-top-left rtl:origin-top-right scale-0 transition duration-300 ease-out rtl:left-0"  role="menu" aria-orientation="vertical" aria-labelledby="dropdown-transform">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>
</div>
```

<!-- Animation items -->

### Animation items

Apply the `dropdown-open:{tw-utility-class}` modifier to introduce animation to your dropdown menu sub container. Also add `data-dropdown-transition` attribute for the sub-container.

The following example demonstrates a translate animation of content.

```html
<div class="w-full">
  <div class="dropdown relative inline-flex [--strategy:absolute]">
    <button id="dropdown-transform" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Dropdown
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <div class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60 rtl:left-0" role="menu" aria-orientation="vertical">
      <ul class="dropdown-open:ease-in dropdown-open:translate-x-0 -translate-x-1 rtl:translate-x-1 transition duration-300 ease-out" aria-labelledby="dropdown-transform" data-dropdown-transition>
        <li><a class="dropdown-item" href="#">My Profile</a></li>
        <li><a class="dropdown-item" href="#">Settings</a></li>
        <li><a class="dropdown-item" href="#">Billing</a></li>
        <li><a class="dropdown-item" href="#">FAQs</a></li>
      </ul>
    </div>
  </div>
</div>
```

<!-------------------- Dropdown state -------------------->

## Dropdown state

<!-- Active state -->

### Active state

Add class `.dropdown-active` to set the active state.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-active" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-active">
    <li><a class="dropdown-item dropdown-active" href="#" aria-current="true">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Disabled state -->

### Disabled state

Add class `.dropdown-disabled` to set the disabled state.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-disabled" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-disabled">
    <li><a class="dropdown-item dropdown-disabled" href="#" aria-disabled="true">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Hover -->

### Hover

The default trigger mode is click, you can change it to hover by adding `[--trigger:hover]` with `dropdown`.

```html
<div class="dropdown relative inline-flex [--trigger:hover]">
  <button id="dropdown-hover" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60 after:h-4 after:absolute after:-bottom-4 after:start-0 after:w-full before:h-4 before:absolute before:-top-4 before:start-0 before:w-full" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-hover">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Dividers -->

### Dividers

The default dropdown menu with dividers.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-dividers" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dividers">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
    <li><hr class="border-base-content/25 -mx-2" /></li>
    <li><a class="dropdown-item" href="#">Pricing</a></li>
    <li><hr class="border-base-content/25 -mx-2" /></li>
    <li><a class="dropdown-item" href="#">Logout Out</a></li>
  </ul>
</div>
```

<!-- Icons -->

### Icons

The standard dropdown menu featuring icons.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-icons" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-icons">
    <li>
      <a class="dropdown-item" href="#">
        <span class="icon-[tabler--bell] size-5 shrink-0"></span>
        My Profile
      </a>
    </li>
    <li>
      <a class="dropdown-item" href="#">
        <span class="icon-[tabler--garden-cart] size-5 shrink-0"></span>
        Settings
      </a>
    </li>
    <li>
      <a class="dropdown-item" href="#">
        <span class="icon-[tabler--cloud-download] size-5 shrink-0"></span>
        Billing
      </a>
    </li>
    <li>
      <a class="dropdown-item" href="#">
        <span class="icon-[tabler--users] size-5 shrink-0"></span>
        FAQs
      </a>
    </li>
  </ul>
</div>
```

<!-- Shortcuts -->

### Shortcuts

The standard dropdown menu with shortcuts using `keyboard` component.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-shortcuts" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-shortcuts">
    <li>
      <a class="dropdown-item justify-between" href="#">
        Dashboard
        <span class>
          <kbd class="kbd kbd-sm">⌘</kbd>
          +
          <kbd class="kbd kbd-sm">i</kbd>
        </span>
      </a>
    </li>
    <li>
      <a class="dropdown-item justify-between" href="#">
        Settings
        <span class>
          <kbd class="kbd kbd-sm">⌘</kbd>
          +
          <kbd class="kbd kbd-sm">s</kbd>
        </span>
      </a>
    </li>
    <li>
      <a class="dropdown-item justify-between" href="#">
        Billing
        <span class>
          <kbd class="kbd kbd-sm">⌘</kbd>
          +
          <kbd class="kbd kbd-sm">d</kbd>
        </span>
      </a>
    </li>
    <li>
      <a class="dropdown-item justify-between" href="#">
        Sign out
        <span class>
          <kbd class="kbd kbd-sm">⌘</kbd>
          +
          <kbd class="kbd kbd-sm">l</kbd>
        </span>
      </a>
    </li>
  </ul>
</div>
```

<!-- Scrollable body -->

### Dropdown with scrollable body

Apply the `overflow-y-auto` class to create a scrollable area, and define the minimum height for this container.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-scrollable" type="button" class="dropdown-toggle" aria-label="Notification Button">
    <div class="indicator">
      <span class="indicator-item bg-error size-2.5 rounded-full"></span>
      <span class="icon-[tabler--bell] text-base-content size-5"></span>
    </div>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-scrollable">
    <div class="dropdown-header justify-center">
      <h6 class="text-base text-base-content">Notification</h6>
    </div>
    <div class="overflow-y-auto text-base-content/80 max-h-52 max-sm:max-w-72">
      <div class="dropdown-item">
        <div class="avatar avatar-away-bottom">
          <div class="w-10 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="truncate text-base">Charles Franklin</h6>
          <small class="text-base-content/50 truncate">Accepted your connection</small>
        </div>
      </div>
      <div class="dropdown-item">
        <div class="avatar">
          <div class="w-10 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="!truncate text-base">Martian added moved Charts & Maps task to the done board.</h6>
          <small class="text-base-content/50 truncate">Today 10:00 AM</small>
        </div>
      </div>
      <div class="dropdown-item">
        <div class="avatar avatar-online-bottom">
          <div class="w-10 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-8.png" alt="User Avatar" />
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="truncate text-base">New Message</h6>
          <small class="text-base-content/50 truncate">You have new message from Natalie</small>
        </div>
      </div>
      <div class="dropdown-item">
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-10 rounded-full p-2">
            <span class="icon-[tabler--user] size-full"></span>
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="truncate text-base">Application has been approved 🚀</h6>
          <small class="text-base-content/50 text-wrap">Your ABC project application has been approved.</small>
        </div>
      </div>
      <div class="dropdown-item">
        <div class="avatar">
          <div class="w-10 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-10.png" alt="User Avatar" />
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="truncate text-base">New message from Jane</h6>
          <small class="text-base-content/50 text-wrap">Your have new message from Jane</small>
        </div>
      </div>
      <div class="dropdown-item">
        <div class="avatar">
          <div class="w-10 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Avatar" />
          </div>
        </div>
        <div class="w-52 sm:w-60">
          <h6 class="truncate text-base">Barry Commented on App review task.</h6>
          <small class="text-base-content/50 truncate">Today 8:32 AM</small>
        </div>
      </div>
    </div>
    <a href="#" class="dropdown-footer justify-center gap-1">
      <span class="icon-[tabler--eye] size-4"></span>
      View all
    </a>
  </div>
</div>
```

<!-- Dropdown input -->

### Dropdown input

With `join` you can combine a dropdown and input into one unit.

> **Info:** Refer the [Join](forms/join/) component documentation for creating a group of buttons.

```html
<div class="join">
  <input class="input join-item" placeholder="Email" />
  <div class="dropdown relative inline-flex w-full">
    <button id="dropdown-input" type="button" class="dropdown-toggle btn btn-primary join-item" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Dropdown
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-input">
      <li><a class="dropdown-item" href="#">Subscribe</a></li>
      <li><a class="dropdown-item" href="#">Verify</a></li>
    </ul>
  </div>
</div>
```

<!-- Destroy/Reinitialize -->

### Destroy/Reinitialize

The `destroy` <a href="#destroy-method" class="link link-primary">method</a> is provided to facilitate the destruction of a dropdown element.

```html
<div id="dropdown-to-destroy" class="dropdown relative inline-flex">
  <button id="dropdown-default" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<div class="mt-4 flex gap-3">
  <button class="btn btn-primary" id="destroy-btn">Destroy</button>
  <button class="btn btn-primary" id="reinit-btn" disabled>Reinitialize</button>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', () => {
    ;(function () {
      const dropdown = document.querySelector('#dropdown-to-destroy')
      const destroy = document.querySelector('#destroy-btn')
      const reinit = document.querySelector('#reinit-btn')

      destroy.addEventListener('click', () => {
        const { element } = HSDropdown.getInstance(dropdown, true)

        element.destroy()

        destroy.setAttribute('disabled', 'disabled')
        reinit.removeAttribute('disabled')
      })

      reinit.addEventListener('click', () => {
        HSDropdown.autoInit()

        reinit.setAttribute('disabled', 'disabled')
        destroy.removeAttribute('disabled')
      })
    })()
  });
</script>
```

<!-------------------- Responsive -------------------->

## Responsive

<!-- Dropdown at sm -->

### Dropright at sm

Apply the <a href="https://tailwindcss.com/docs/hover-focus-and-other-states#responsive-breakpoints" class="link link-primary" target="_blank" >Responsive modifier</a> to adapt the dropdown position across different viewport sizes.

For instance, for below example the initial position is set to bottom-start, and it changes to right-start above the 'sm' breakpoint.

```html
<div class="dropdown relative inline-flex [--placement:right-start]">
  <button id="dropdown-sm" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" aria-labelledby="dropdown-sm">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-------------------- Options usage -------------------->

## Options usage

<!-- Auto close behavior -->

### Auto close behavior

> **Info:** We are using <a href="https://floating-ui.com/" class="link link-primary" target="_blank">FloatingUI</a> library for dropdown and tooltip.

By default, clicking inside or outside the dropdown menu will close it. You can modify this behavior using the `[--auto-close:"true(DEFAULT) | inside | outside | false"]` option.

- `true`: The dropdown closes when clicked both inside and outside.
- `inside`: Allow click inside dropdown mainly for input component.
- `outside`: Allow click outside dropdown.
- `false`: The dropdown only closes when the button is clicked.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-outside" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    True (DEFAULT)
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-outside">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--auto-close:inside]">
  <button id="dropdown-transportation" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Inside
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <div class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-transportation">
    <div class="dropdown-item gap-4">
      <input id="dropdown-radio-car" name="dropdown-item-radio-2" type="radio" class="radio radio-primary" checked/>
      <label for="dropdown-radio-car" class="label-text text-base-content block text-sm font-semibold">Car </label>
    </div>
    <div class="dropdown-item gap-4">
      <input id="dropdown-radio-bicycle" name="dropdown-item-radio-2" type="radio" class="radio radio-primary" />
      <label for="dropdown-radio-bicycle" class="label-text text-base-content text-sm font-semibold"> Bicycle </label>
    </div>
  </div>
</div>

<div class="dropdown relative inline-flex [--auto-close:outside]">
  <button id="dropdown-outside" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Outside
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-outside">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--auto-close:false]">
  <button id="dropdown-false" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    False
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-false">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Strategy -->

### Strategy

By default, the `strategy` is set to 'fixed'. To switch it to 'absolute', use the `[--strategy:*]` option.

```html
<div class="w-full">
  <div class="dropdown relative inline-flex [--strategy:absolute]">
    <button id="dropdown-strategy" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Dropdown
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60 rtl:left-0" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-strategy">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>
</div>
```

<!-- Offset -->

### Offset

Use `[--offset:*]` to set the number of pixels you want the dropdown menu to be offset from the trigger element.

```html
<div class="dropdown relative inline-flex [--offset:30]">
  <button id="dropdown-offset" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-offset">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- No flip -->

### No flip

If you prefer to disable the automatic positioning of the `dropdown-menu`.

```html
<div class="dropdown relative inline-flex [--flip:false]">
  <button id="dropdown-flip" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-flip">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

<!-- Direction -->

### Direction

By default the dropdown direction is bottom-start. To change it use `[--placement:*]`. For centered use simple `top`, `bottom`, `right`, `left` direction.

<!-- Dropup -->

#### Dropup

Use `[--placement:top | top-start | top-end]` class to trigger dropup menus above elements.

```html
<div class="dropdown relative inline-flex [--placement:top-start]">
  <button id="dropdown-dropup-start" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Top start
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropup-start">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:top]">
  <button id="dropdown-dropup" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Top
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropup">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:top-end]">
  <button id="dropdown-dropup-end" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Top end
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropup-end">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>
```

#### Dropdown

Use `[--placement:bottom | bottom-start(DEFAULT) | bottom-end]` class to trigger dropdown menus above elements.

```html
<div class="dropdown relative inline-flex">
  <button id="dropdown-bottom-start" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Bottom start
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-bottom-start">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:bottom]">
  <buttom id="dropdown-bottom" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Bottom
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </buttom>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-bottom">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:bottom-end]">
  <button id="dropdown-bottom-start" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Bottom end
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-bottom-start">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>
```

<!-- Dropright -->

#### Dropright

Use `[--placement:right | right-start | right-end]` class to trigger dropright menus above elements.

```html
<div class="flex flex-col gap-9">
  <div class="dropdown relative inline-flex [--placement:right-start]">
    <button id="dropdown-dropright-start" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Right start
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropright-start">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>

  <div class="dropdown relative inline-flex [--placement:right]">
    <buttom id="dropdown-dropright" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Right
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </buttom>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropright">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>

  <div class="dropdown relative inline-flex [--placement:right-end]">
    <button id="dropdown-dropright-end" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Right end
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropright-end">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>
</div>
```

<!-- Dropleft -->

#### Dropleft

Use `[--placement:left | left-start | left-end]` class to trigger dropleft menus above elements.

```html
<div class="dropdown relative inline-flex [--placement:left-start]">
  <button id="dropdown-dropleft-start" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Left start
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropleft-start">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:left]">
  <buttom id="dropdown-dropleft" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Left
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </buttom>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropleft">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>

<div class="dropdown relative inline-flex [--placement:left-end]">
  <button id="dropdown-dropleft-end" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Left end
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dropleft-end">
    <li><a class="dropdown-item" href="#"> My Profile </a></li>
    <li><a class="dropdown-item" href="#"> Settings </a></li>
    <li><a class="dropdown-item" href="#"> Billing </a></li>
    <li><a class="dropdown-item" href="#"> FAQs </a></li>
  </ul>
</div>
```

<!-------------------- Accessibility notes -------------------->

## Accessibility notes

<!-- Keyboard interDropdown -->

### Keyboard interactions

<!-- interDropdown table -->

{{< table >}}
COMMAND| DESCRIPTION
<kbd class="kbd kbd-sm">Enter</kbd>| Activates the selected tab.

<div class="flex gap-3"><kbd class="kbd kbd-sm">A-Z</kbd> <kbd class="kbd kbd-sm">a-z</kbd></div>| Focuses first item that matches keyboard input.
<div class="flex gap-3"><kbd class="kbd kbd-sm">Home</kbd> <kbd class="kbd kbd-sm">End</kbd></div>| Focuses first/last non-disabled item.
<kbd class="kbd kbd-sm">Esc</kbd>| Closes any open Menus.
<div class="flex gap-3"><kbd class="kbd"><span class="icon-[tabler--caret-up-filled] size-5"></span></kbd> <kbd class="kbd"><span class="icon-[tabler--caret-down-filled] size-5"></span></kbd></div>| Focuses previous/next non-disabled item.
{{< /table >}}

<!-------------------- JavaScript behavior -------------------->

## JavaScript behavior

<!-- Options -->

### Options

> **Info:** FlyonUI is powered by <a href="https://preline.co/plugins/html/dropdown.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

<!-- Options table -->

{{< table >}}

PARAMETERS|DESCRIPTION|OPTIONS|DEFAULT VALUE
<span class="text-nowrap">`data-dropdown-transition`</span>| <span class="text-pretty">A data attribute is used to specify the container that will undergo animation.</span>|`-`|`-`
<span colspan="4" class="text-base-content font-semibold">Class Options</span>
`[--placement:*]`|Defines the menu's position upon opening.| top, top-start, top-end, bottom, bottom-start, bottom-end, right, right-start, right-end, left, left-start, left-end|<span class="text-nowrap">`bottom-start`</span>
`[--scope:*]`|Determines whether the dropdown will be moved outside the parent, for correct display in elements with hidden overflow. Requires the <code>Floating UI</code>plugin.| window, parent|<span class="text-nowrap">`parent`</span>
`[--auto-close:*]`|Disables autofocus on the first focusable element when opening a dropdown. Should be added to the <span class="font-medium">container (.dropdown)</span>.|inside, outside, false, true|`true`
`[----has-autofocus:*]`|Specifies the area where clicking is allowed.|true, false|`true`
`[--strategy:*]`|Indicates the area that, when clicked, will trigger the menu to close.|fixed, absolute|`fixed`
`[--offset:*]`|Adjusts the dropdown's offset from the bottom or top.|number|`5`
`[--gpu-acceleration:*]`|Disable/enable position calculation using the transform property. Should be added to the <span class="font-medium">container (.dropdown)</span>.|true, false|`true`
`[--flip:*]`|Changes the menu's position to prevent overlapping with its reference element.|true, false| `true`
`[--trigger:*]`|Event to trigger a dropdown| hover , click |`click`
{{< /table >}}

<!-- Methods -->

### Methods

The `HSDropdown` object is contained within the global `window` object.

{{< table >}}
METHOD|DESCRIPTION
<span colspan="2" class="text-base-content font-semibold">PUBLIC METHODS</span>
`open()`| Opens the dropdown menu forcefully.
`close(isAnimated)`| <div>Closes the dropdown menu forcefully.<ul class="m-0"><li><code>isAnimated boolean:</code> Indicates if the dropdown menu should close with animation.</li></ul></div>
`forceClearState()`|Completely removes the dropdown.
`destroy()`| Destroys the instance, removes generated markup (if any), removes added classes and attributes.
<span colspan="2" class="text-base-content font-semibold">STATIC METHODS</span>
`HSDropdown.getInstance(target)`|<div>Retrieves the element associated with the <code>target</code>.<ul class="m-0"><li>The <code>target</code> can be either a Node or a string (a valid CSS selector).</li></ul></div>
`HSDropdown.open(target)`|<div>Forces the dropdown menu to open.<ul class="m-0"><li>The <code>target</code> must be a Node.</li></ul></div>
`HSDropdown.close(target)`|<div>Forces the dropdown menu to close.<ul class="m-0"><li>The <code>target</code> must be a Node.</li></ul></div>
{{< /table >}}

<!-- Method usage -->

#### Method usage

Below, is the demonstration on how to use the public methods. Apply the ID to the `dropdown` component class. To test other methods, copy the following methods into your console and click the button.

```html
<div class="flex gap-10 flex-wrap">
  <div class="dropdown relative inline-flex --prevent-on-load-init" id="dropdown-method">
    <button id="dropdown-method-usage" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Dropdown
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-method-usage">
      <li><a class="dropdown-item" href="#">My Profile</a></li>
      <li><a class="dropdown-item" href="#">Settings</a></li>
      <li><a class="dropdown-item" href="#">Billing</a></li>
      <li><a class="dropdown-item" href="#">FAQs</a></li>
    </ul>
  </div>

<button class="btn btn-primary" id="open-btn">Method</button>

</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    const dropdown = new HSDropdown(document.querySelector('#dropdown-method'))
    const openBtn = document.querySelector('#open-btn')

    openBtn.addEventListener('click', () => {
      dropdown.open()
    })
  })
</script>
```

<p class="mt-10 mb-1.5 not-prose">Open item (public method).</p>

```js
// This method is used in above example.
const dropdown = new HSDropdown(document.querySelector('#dropdown-method'));
const openBtn = document.querySelector('#open-btn');

openBtn.addEventListener('click', () => {
  dropdown.open();
});
```

<p class="mb-1.5 not-prose">Open item (static method).</p>

```js
const openBtn = document.querySelector('#open-btn');

openBtn.addEventListener('click', () => {
  HSDropdown.open('#dropdown-method');
});
```

<p class="mb-1.5 not-prose">Open item (mixed).</p>

```js
const { element } = HSDropdown.getInstance('#dropdown-method', true);
const openBtn = document.querySelector('#open-btn');

openBtn.addEventListener('click', () => {
  element.open();
});
```

<p class="mb-1.5 not-prose" id="destroy-method">Destroy instance (public).</p>

```js
const dropdown = document.querySelector('#dropdown-to-destroy')
const destroy = document.querySelector('#destroy-btn')

destroy.addEventListener('click', () => {
  const { element } = HSDropdown.getInstance(dropdown, true)
  element.destroy()
})
```

<!-- Events -->

### Events

{{< table >}}
METHOD| DESCRIPTION
`on:open`|Triggered whenever a dropdown menu is opened.
`on:close`|Triggered whenever a dropdown menu is closed.
{{< /table >}}

<!-- Event usage -->

#### Event usage

Below, is the demonstration on how to use the event. Apply the ID to the `dropdown` component class. To test these event, copy the following event into your console and click the button.

```html
<div class="dropdown relative inline-flex" id="dropdown-event">
  <button id="dropdown-event-usage" type="button" class="dropdown-toggle btn btn-primary" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
    Dropdown
    <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
  </button>
  <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-event-usage">
    <li><a class="dropdown-item" href="#">My Profile</a></li>
    <li><a class="dropdown-item" href="#">Settings</a></li>
    <li><a class="dropdown-item" href="#">Billing</a></li>
    <li><a class="dropdown-item" href="#">FAQs</a></li>
  </ul>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    const { element } = HSDropdown.getInstance('#dropdown-event', true)

    element.on('open', instance => {
      console.log('open')
    })
    element.on('close', instance => {
      console.log('close')
    })
  })
</script>
```

<p class="mt-12 mb-1.5 not-prose">Open any dropdown event example.</p>

```js
const { element } = HSDropdown.getInstance('#dropdown-event', true)

element.on('open', (instance) => {console.log("open")});
element.on('close', (instance) => {console.log("close")});
```
