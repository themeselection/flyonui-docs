# Input 

A fundamental tool for receiving user input is a text field, which allows data to be provided or altered using either the keyboard or mouse.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| input | component | Base class for form input. |
| input-floating | component | Base class for floating form input. |
| input-floating-label | part | Floats the label to the top. |
| label-text | part | Base class for title label text. |
| helper-text | part | Base class for helper label text. |
| no-focus | modifier | remove default focus from input. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| input-xs | size | Input with Extra small size. |
| input-sm | size | Input with Smaller size. |
| input-md | size | Input with medium(default) size. |
| input-lg | size | Input with Larger size. |
| input-xl | size | Input with Extra large size. |


<!-------------------- Basic example -------------------->

## Basic examples

<!-- Default -->

### Default

Utilize the `input` component class to style the input.

```html
<input type="text" class="input max-w-sm" aria-label="input" />
```

<!-- Placeholder -->

### Placeholder

Basic input with placeholder.

```html
<input type="text" placeholder="Type here" class="input max-w-sm" />
```

<!-- Label and helper text -->

### Label and helper text

Please use `label-text` for the label and `helper-text` for the text that appears at the bottom as helper text.

```html
<div class="w-96">
  <label class="label-text" for="labelAndHelperText">Full Name</label>
  <input type="text" placeholder="John Doe" class="input" id="labelAndHelperText" />
  <span class="helper-text">Please write your full name</span>
</div>

<div class="w-96">
  <label class="label-text" for="labelAndHelperTextRight">Full Name</label>
  <input type="text" placeholder="John Doe" class="input" id="labelAndHelperTextRight" />
  <span class="helper-text text-end">Please write your full name</span>
</div>
```

<!-- Hidden label -->

### Hidden label

`label` elements hidden using the `.sr-only` class.

```html
<div class="w-96">
  <label class="label-text sr-only" for="hiddenLabel">Full name</label>
  <input type="text" id="hiddenLabel" class="input" placeholder="John Doe" />
</div>
```

<!-------------------- Types -------------------->

## Types

<!-- Default -->

### Default

Default Input.

```html
<div class="w-96">
  <label class="label-text" for="defaultInput">Full name</label>
  <input type="text" placeholder="John Doe" class="input" id="defaultInput" />
</div>
```

<!-- Floating label -->

### Floating label

The **Floating Input Component** provides a text input with a floating label. Use `.input-floating` for the wrapper, `.input` for the input field, and `.input-floating-label` for the label.

```html
<div class="input-floating w-96">
  <input type="text" placeholder="John Doe" class="input" id="floatingInput" />
  <label class="input-floating-label" for="floatingInput">Full name</label>
</div>
```


<!-------------------- Size -------------------->

## Sizes

<!-- Default -->

### Default

Add responsive class `input-{size}` where `{size} = xs|sm|md|lg|xl` for input of different sizes.

```html
<input type="text" placeholder="John Doe" class="input input-xs max-w-sm" />
<input type="text" placeholder="John Doe" class="input input-sm max-w-sm" />
<input type="text" placeholder="John Doe" class="input max-w-sm" />
<input type="text" placeholder="John Doe" class="input input-lg max-w-sm" />
<input type="text" placeholder="John Doe" class="input input-xl max-w-sm" />
```

<!-- Floating label -->

### Floating label

Add responsive class `input-{size}` where `{size} = xs|sm|md|lg|xl` for input of different sizes for floating label.

```html
<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input input-xs" id="floatingLabelExtraSmall" />
  <label class="input-floating-label" for="floatingLabelExtraSmall">Full name</label>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input input-sm" id="floatingLabelSmall" />
  <label class="input-floating-label" for="floatingLabelSmall">Full name</label>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input" id="floatingLabelDefault" />
  <label class="input-floating-label" for="floatingLabelDefault">Full name</label>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input input-lg" id="floatingLabelLarge" />
  <label class="input-floating-label" for="floatingLabelLarge">Full Name</label>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input input-xl" id="floatingLabelExtraLarge" />
  <label class="input-floating-label" for="floatingLabelExtraLarge">Full Name</label>
</div>
```

<!-------------------- Validation State -------------------->

## Validation State

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="successInput">Full Name</label>
  <input type="text" placeholder="John Doe" class="input is-valid" id="successInput" />
  <span class="helper-text">Helper text</span>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input is-valid" id="successFloatingInput" />
  <label class="input-floating-label" for="successFloatingInput">Full name</label>
  <span class="helper-text ps-3">Helper text</span>
</div>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="errorInput">Full Name</label>
  <input type="text" placeholder="John Doe" class="input is-invalid" id="errorInput" />
  <span class="helper-text">Helper text</span>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input is-invalid" id="errorFloatingInput" />
  <label class="input-floating-label" for="errorFloatingInput">Full name</label>
  <span class="helper-text ps-3">Helper text</span>
</div>
```

<!-------------------- Input Group -------------------->

## Input Group

<!-- Inline label -->

### Inline label

To create an input group, use `input` as a wrapper. To align the `label` or `icons`, apply the `my-auto` class. This ensures consistent vertical alignment within the group.

```html
<div class="input max-w-sm">
  <label class="label-text my-auto me-3 p-0" for="inlineLabelName">Name</label>
  <input type="text" class="grow" placeholder="FlyonUI" id="inlineLabelName" />
</div>
<div class="input max-w-sm">
  <label class="label-text my-auto me-3 p-0" for="inlineLabelEmail">Email</label>
  <input type="email" class="grow" placeholder="admin@site.com" id="inlineLabelEmail" />
</div>
```

<!-- Leading icon -->

### Leading icon

Add a leading icon inside input.

```html
<div class="input max-w-sm">
  <span class="icon-[tabler--user] text-base-content/80 my-auto me-3 size-5 shrink-0"></span>
  <label class="sr-only" for="leadingIconDefault">Full Name</label>
  <input type="text" class="grow" placeholder="John Doe" id="leadingIconDefault" />
</div>

<div class="input max-w-sm">
  <span class="icon-[tabler--user] text-base-content/80 my-auto size-5 shrink-0"></span>
  <div class="input-floating grow">
    <input type="text" placeholder="John Doe" class="ps-3" id="leadingIconFloating" />
    <label class="input-floating-label" for="leadingIconFloating">Full name</label>
  </div>
</div>
```

<!-- Trailing icon -->

### Trailing icon

Add a trailing icon inside input.

```html
<div class="input max-w-sm">
  <input type="text" class="grow" placeholder="xxxx-xxxx-xxxx-xxxx" id="trailingIconDefault" />
  <label class="sr-only" for="trailingIconDefault">Card Number</label>
  <span class="icon-[tabler--brand-mastercard] text-base-content/80 my-auto ms-3 size-5 shrink-0"></span>
</div>

<div class="input max-w-sm">
  <div class="input-floating grow">
    <input type="text" class="grow" placeholder="xxxx-xxxx-xxxx-xxxx" id="trailingIconFloating" />
    <label class="input-floating-label ms-0" for="trailingIconFloating">Full name</label>
  </div>
  <span class="icon-[tabler--brand-mastercard] text-base-content/80 my-auto ms-3 size-5 shrink-0"></span>
</div>
```

<!-- Leading and trailing icon -->

### Leading and trailing icon

Add a leading and trailing icon inside input.

```html
<div class="input max-w-sm space-x-3">
  <span class="label-text my-auto">$</span>
  <input type="number" class="grow" placeholder="00.00" id="trailingAndLeadingInput" />
  <label class="sr-only" for="trailingAndLeadingInput">Enter amount</label>
  <span class="label-text my-auto">USD</span>
</div>
```

<!-- With keyboard shortcut -->

### With keyboard shortcut

Utilizes `kbd` component class with input.

```html
<div class="input input-lg flex max-w-sm space-x-4">
  <span class="icon-[tabler--search] text-base-content/80 my-auto size-6 shrink-0"></span>
  <input type="search" class="grow" placeholder="Search" id="kbdInput" />
  <label class="sr-only" for="kbdInput">Search</label>
  <span class="my-auto flex gap-2">
    <kbd class="kbd kbd-sm">⌘</kbd>
    <kbd class="kbd kbd-sm">K</kbd>
  </span>
</div>
```

<!-- Checkbox and radios -->

### Checkbox and radios

Place any checkbox or radio option within an input group’s addon instead of text.

```html
<div class="input max-w-sm">
  <input type="checkbox" class="checkbox checkbox-primary my-auto me-3" />
  <input type="text" class="grow" placeholder="John Doe" />
</div>

<div class="input max-w-sm">
  <input type="radio" name="radio-1" class="radio radio-primary my-auto me-3" />
  <input type="text" class="grow" placeholder="John Doe" />
</div>
```

<!-- Inline select -->
### Inline select

This example demonstrates an inline select component. The `.input` class serves as a wrapper, incorporating `pe-0` for padding reset and `items-center` for vertical alignment. Additionally, `ms-3` is used to manage spacing.  


```html
<div class="input items-center pe-0 max-w-sm">
  <input class="grow" placeholder="Search" />
  <select class="select ms-3" aria-label="select">
    <option disabled selected>Filter</option>
    <option>Sci-fi</option>
    <option>Drama</option>
    <option>Action</option>
  </select>
</div>
```

<!-------------------- Shape -------------------->

## Shape

<!-- Pill input -->

### Pill input

We can manage the input's radius using the <a href="https://tailwindcss.com/docs/border-radius" target="_blank" class="link link-primary">rounded</a> utility class provided by Tailwind CSS.


```html
<div class="max-w-sm">
  <label class="label-text" for="pillInput">Full Name</label>
  <input type="text" placeholder="John Doe" class="input rounded-full" id="pillInput" />
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input rounded-full" id="pillFloatingInput" />
  <label class="input-floating-label" for="pillFloatingInput">Full name</label>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Helper text -->

### Helper text

Implement varying input styles accompanied by helper text.

```html
<div class="space-y-3">
  <div class="relative">
    <label class="label-text" for="helperTextInput">Full Name</label>
    <input type="text" placeholder="John Doe" class="input max-w-sm" id="helperTextInput" />
    <span class="helper-text">Please write your full name</span>
  </div>

  <div class="input-floating max-w-sm">
    <input type="text" placeholder="John Doe" class="input" id="helperTextFloatingInput" />
    <label class="input-floating-label" for="helperTextFloatingInput">Full Name</label>
    <span class="helper-text ps-3">Please write your full name</span>
  </div>
</div>
```

<!-- No focus -->

### No focus

Disable the default focus on the `input` using `no-focus` class when necessary.

```html
<input type="text" placeholder="Type here" class="input no-focus border-0 max-w-sm" />
```


<!-- Disabled -->

### Disabled

Add the `disabled` boolean attribute on an input to remove pointer events, and prevent focusing.

```html
<div class="w-96">
  <label class="label-text" for="disabledInput"> What is your name? </label>
  <input type="text" placeholder="John Doe" class="input" id="disabledInput" disabled />
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input" id="disabledFloatingInput" disabled/>
  <label class="input-floating-label" for="disabledFloatingInput">Full Name</label>
</div>
```

<!-- Readonly -->

### Readonly

Add the `readonly` boolean attribute on an input to prevent modification of the input’s value.

```html
<div class="w-96">
  <label class="label-text" for="readonlyInput">What is your name?</label>
  <input type="text" placeholder="John Doe" class="input" id="readonlyInput" readonly />
</div>
```

<!-------------------- Join -------------------->

## Join

<!-- Input with button -->

### Input with button

Combine a button with the input field using the `join` method.

> **Info:** Use [Join](forms/join/) component to combine two components, like an input with a button, button groups, or an input paired with a dropdown.

```html
<div class="join max-w-sm">
  <input class="input join-item" placeholder="Search" />
  <button class="btn btn-outline btn-secondary join-item">Search</button>
</div>

<div class="join max-w-sm">
  <button class="btn btn-outline btn-secondary join-item">Search</button>
  <input class="input join-item" placeholder="Search" />
</div>
```

<!-- Input group with button -->

### Input group with button

Combine a button with the input input.

```html
<div class="join w-96">
  <div class="input join-item flex">
    <span class="icon-[tabler--user] text-base-content/80 my-auto me-3 size-5 shrink-0"></span>
    <label class="sr-only" for="groupInput">Full Name</label>
    <input type="text" class="grow" placeholder="John Doe" id="groupInput" />
  </div>
  <button class="btn btn-outline btn-secondary join-item h-auto">Search</button>
</div>
```

<!-- Input with select -->

### Input with select

Combine a select with the input input.

```html
<div class="join w-96">
  <input class="input join-item" placeholder="Search" />
  <select class="select join-item w-36" aria-label="select">
    <option disabled selected>Filter</option>
    <option>Sci-fi</option>
    <option>Drama</option>
    <option>Action</option>
  </select>
</div>
```
