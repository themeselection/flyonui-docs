# Textarea

A textarea is a multi-line input field that enables users to enter longer blocks of text, such as comments, messages, or descriptions.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| textarea | component | Basic textarea field. |
| textarea-floating | component | Floating textarea field. |
| textarea-floating-label | part | Floats the label to the top. |
| label-text | part | For label. |
| helper-text | part | For helper text. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| textarea-xs | size | Extra small Textarea size. |
| textarea-sm | size | Smaller Textarea size. |
| textarea-md | size | Medium(default) Textarea size. |
| textarea-lg | size | Larger Textarea size. |
| textarea-xl | size | Extra large Textarea size. |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic textarea example.

```html
<textarea class="textarea max-w-sm" aria-label="Textarea" ></textarea>
```

<!-- Label and placeholder -->

### Label and placeholder

Basic textarea with placeholder.

```html
<div class="sm:w-96">
  <label class="label-text" for="textareaLabel"> Your bio </label>
  <textarea class="textarea" placeholder="Hello!!!" id="textareaLabel"></textarea>
</div>
```

<!-------------------- Type -------------------->

## Types

<!-- Default -->

### Default

```html
<textarea class="textarea max-w-sm" placeholder="Hello!!!" ></textarea>
```

<!-- Floating label -->

### Floating label

The `textarea-floating` style is used to define the appearance of the textarea, while the `textarea-floating-label` is the container for the label text.

```html
<div class="textarea-floating sm:w-96">
  <textarea class="textarea" placeholder="Hello!!!" id="textareaFloating"></textarea>
  <label class="textarea-floating-label" for="textareaFloating">Your bio</label>
</div>
```

<!-------------------- Size -------------------->

## Size

<!-- Default -->

### Default

Add responsive class `textarea-{size}` where `{size} = xs|sm|md|lg|xl` for textarea of different sizes.

```html
<textarea class="textarea textarea-xs max-w-sm" placeholder="Hello!!!" ></textarea>

<textarea class="textarea textarea-sm max-w-sm" placeholder="Hello!!!" ></textarea>

<textarea class="textarea max-w-sm" placeholder="Hello!!!" ></textarea>

<textarea class="textarea textarea-lg max-w-sm" placeholder="Hello!!!" ></textarea>

<textarea class="textarea textarea-xl max-w-sm" placeholder="Hello!!!" ></textarea>
```

<!-- Floating label -->

### Floating label

Add responsive class `select-{size}` where `{size} = xs|sm|md|lg|xl` for select of different sizes.

```html
<div class="textarea-floating sm:w-96">
  <textarea class="textarea textarea-xs" placeholder="Hello!!!" id="textareaFloatingExtraSmall"></textarea>
  <label class="textarea-floating-label" for="textareaFloatingExtraSmall">Your bio</label>
</div>

<div class="textarea-floating sm:w-96">
  <textarea class="textarea textarea-sm" placeholder="Hello!!!" id="textareaFloatingSmall"></textarea>
  <label class="textarea-floating-label" for="textareaFloatingSmall">Your bio</label>
</div>

<div class="textarea-floating sm:w-96">
  <textarea class="textarea" placeholder="Hello!!!" id="textareaFloatingMedium"></textarea>
  <label class="textarea-floating-label" for="textareaFloatingMedium">Your bio</label>
</div>

<div class="textarea-floating sm:w-96">
  <textarea class="textarea textarea-lg" placeholder="Hello!!!" id="textareaFloatingLarge"></textarea>
  <label class="textarea-floating-label" for="textareaFloatingLarge">Your bio</label>
</div>

<div class="textarea-floating sm:w-96">
  <textarea class="textarea textarea-xl" placeholder="Hello!!!" id="textareaFloatingExtraLarge"></textarea>
  <label class="textarea-floating-label" for="textareaFloatingExtraLarge">Your bio</label>
</div>
```

<!-------------------- Textarea group -------------------->
## Textarea group

<!-- Leading icons -->

### Leading icons

Add a leading icon inside textarea.

```html
<div class="textarea max-w-sm">
  <span class="icon-[tabler--message] text-base-content/80 mt-2 mx-4 size-5 shrink-0"></span>
  <textarea class="grow" placeholder="Hello!!!"></textarea>
</div>

<div class="textarea max-w-sm">
  <span class="icon-[tabler--message] text-base-content/80 mt-2 mx-4 size-5 shrink-0"></span>
  <div class="textarea-floating grow">
    <textarea placeholder="Hello!!!" id="textareaFloatingMedium"></textarea>
    <label class="textarea-floating-label" for="textareaFloatingMedium">Your bio</label>
  </div>
</div>
```

<!-- Tailing icons -->

### Tailing icons

Add a tailing icon inside textarea.

```html
<div class="textarea max-w-sm">
  <textarea class="grow resize-none" placeholder="Hello!!!"></textarea>
  <span class="icon-[tabler--message] text-base-content/80 mt-2 mx-4 size-5 shrink-0"></span>
</div>

<div class="textarea max-w-sm">
  <div class="textarea-floating grow">
    <textarea class="resize-none" placeholder="Hello!!!" id="textareaFloatingMedium"></textarea>
    <label class="textarea-floating-label" for="textareaFloatingMedium">Your bio</label>
  </div>
  <span class="icon-[tabler--message] text-base-content/80 mt-2 mx-4 size-5 shrink-0"></span>
</div>
```


<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<!-- Basic -->

<div class="sm:w-96">
  <label class="label-text" for="textareaStateSuccessDefault"> Full Name </label>
  <textarea class="textarea is-valid" placeholder="Hello!!!" id="textareaStateSuccessDefault"></textarea>
  <span class="helper-text">Helper text</span>
</div>

<!-- Floating -->

<div class="textarea-floating sm:w-96">
  <textarea class="textarea is-valid" placeholder="Hello!!!" id="textareaStateSuccessFloating"></textarea>
  <label class="textarea-floating-label" for="textareaStateSuccessFloating">Your bio</label>
  <span class="helper-text">Helper text</span>
</div>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<!-- Basic -->

<div class="sm:w-96">
  <label class="label-text" for="textareaStateErrorDefault"> Full Name </label>
  <textarea class="textarea is-invalid" placeholder="Hello!!!" id="textareaStateErrorDefault"></textarea>
  <span class="helper-text">Helper text</span>
</div>

<!-- Floating -->

<div class="textarea-floating sm:w-96">
  <textarea class="textarea is-invalid" placeholder="Hello!!!" id="textareaStateErrorFloating"></textarea>
  <label class="textarea-floating-label" for="textareaStateErrorFloating">Your bio</label>
  <span class="helper-text">Helper text</span>
</div>
```

<!-------------------- Illustration -------------------->

## Illustrations

<!-- Hidden label -->

### Hidden label

`label` elements hidden using the .sr-only class.

```html
<div class="w-full sm:w-96">
  <label class="label-text sr-only" for="textareaHiddenLabel"> Your bio </label>
  <textarea class="textarea" placeholder="Hello!!!" id="textareaHiddenLabel"></textarea>
</div>
```

<!-- Disable -->

### Disable

Add the `disabled` boolean attribute on an textarea to remove pointer events, and prevent focusing.

```html
<div class="w-full sm:w-96">
  <label class="label-text sr-only" for="textareaDisabledefault"> Your bio </label>
  <textarea class="textarea" placeholder="Hello!!!" id="textareaDisabledefault" disabled></textarea>
</div>

<div class="textarea-floating sm:w-96">
  <textarea class="textarea" placeholder="Hello!!!" id="textareaDisabledoating" disabled></textarea>
  <label class="textarea-floating-label" for="textareaDisabledoating">Your bio</label>
</div>
```

<!-- Readonly -->

### Readonly

Add the `readonly` boolean attribute on an textarea to prevent modification of the textarea value.

```html
<div class="w-full sm:w-96">
  <label class="label-text sr-only" for="textareaReadonly"> Your bio </label>
  <textarea class="textarea" placeholder="Hello!!!" id="textareaReadonly" readonly></textarea>
</div>
```

<!-- Helper text -->

### Helper text

Basic textarea example with helper text and hints.

```html
<!-- Basic -->
<div class="w-full sm:w-96">
  <label class="label-text" for="textareaHelperTextDefault"> Full Name </label>
  <textarea class="textarea" placeholder="Hello!!!" id="textareaHelperTextDefault"></textarea>
  <span class="helper-text">Helper text</span>
</div>

<!-- Floating -->
<div class="textarea-floating sm:w-96">
  <textarea class="textarea" placeholder="Hello!!!" id="textareaHelperTextFloating"></textarea>
  <label class="textarea-floating-label" for="textareaHelperTextFloating">Your bio</label>
  <span class="helper-text">Helper text</span>
</div>
```
