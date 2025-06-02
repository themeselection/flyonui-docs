# Input Number

The Input Number, or Quantity Selector, lets users specify quantities easily, making it ideal for selecting product amounts or seats with simple controls.

> **Info:** Input number components are adopted from <a href="https://preline.co/docs/input-number.html" target="_blank" class="link link-primary font-semibold">Preline UI</a> components using <a href="https://preline.co/plugins.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

<!-- Class Table -->

| Class | Type | Description |
| --- | --- | --- |
| input | component | Basic input field. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| input-number-disabled:{tw-utility-class} | variant | The modifier allows setting Tailwind classes when input's value is set to zero. |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic example of input number.

Enclose the `data-input-number-input` and `data-input-number-decrement` elements of the input-number within `data-input-number-increment` within `data-input-number`.

```html
<div class="input max-w-sm" data-input-number>
  <input type="text" value="1" aria-label="Input number" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Label -->

### Label

Input number with label.

```html
<div class="max-w-sm" data-input-number>
  <label class="label-text" for="number-input-label">Quantity:</label>
  <div class="input">
    <input type="text" value="1" aria-label="Label input number" data-input-number-input id="number-input-label" />
    <span class="my-auto flex gap-3">
      <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
        <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
      </button>
      <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
        <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
      </button>
    </span>
  </div>
</div>
```

<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="input max-w-sm" data-input-number>
  <input type="text" class="is-valid" type="text" value="1" aria-label="success state" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="input max-w-sm" data-input-number>
  <input type="text" class="is-invalid" type="text" value="1" aria-label="error state" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Disabled -->

### Disabled

Basic disabled state.

```html
<div class="input max-w-sm" data-input-number>
  <input type="text" type="text" value="1" aria-label="Disable input number" data-input-number-input disabled />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Vertically stacked buttons -->

### Vertically stacked buttons

Vertically stacked buttons example.

```html
<div class="max-w-sm" data-input-number>
  <label class="label-text" for="number-input-vertically">Quantity:</label>
  <div class="input pe-0">
    <input type="text" value="0" aria-label="Vertical stacked buttons" data-input-number-input id="number-input-vertically" />
    <span class="divide-base-content/25 border-base-content/25 my-auto flex flex-col divide-y border-s">
      <button type="button" class="flex size-4.5 items-center justify-center" aria-label="Increment button" data-input-number-decrement >
        <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
      </button>
      <button type="button" class="flex size-4.5 items-center justify-center" aria-label="Decrement button" data-input-number-increment >
        <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
      </button>
    </span>
  </div>
</div>
```

<!-- Horizontally stacked buttons -->

### Horizontally stacked buttons

Horizontally stacked buttons example.

```html
<div class="max-w-sm" data-input-number>
  <label class="label-text" for="number-input-horizontally">Quantity:</label>
  <div class="input pe-0">
    <input type="text" value="0" aria-label="Horizontal stacked buttons" data-input-number-input id="number-input-horizontally" />
    <span class="divide-base-content/25 border-base-content/25 flex items-center divide-x border-s" >
      <button type="button" class="flex size-9.5 items-center justify-center" aria-label="Increment button" data-input-number-decrement >
        <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
      </button>
      <button type="button" class="flex size-9.5 items-center justify-center" aria-label="Decrement button" data-input-number-increment >
        <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
      </button>
    </span>
  </div>
</div>
```

<!-- Horizontally stretched buttons. -->

### Horizontally stretched buttons.

Horizontally stretched buttons example.

```html
<div class="max-w-sm" data-input-number>
  <label class="label-text" for="number-input-stretched">Quantity:</label>
  <div class="input px-0">
    <span class="border-base-content/25 border-e ps-0">
      <button type="button" class="flex size-9.5 items-center justify-center" aria-label="Decrement button" data-input-number-decrement >
        <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
      </button>
    </span>
    <input class="px-3" type="text" value="0" aria-label="Stretched stacked buttons" data-input-number-input id="number-input-stretched" />
    <span class="border-base-content/25 border-s pe-0">
      <button type="button" class="flex size-9.5 items-center justify-center" aria-label="Increment button" data-input-number-increment >
        <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
      </button>
    </span>
  </div>
</div>
```

<!-- Mini  -->

### Mini

Here's a simple example: demonstrate setting a maximum width for the main container.

```html
<div class="max-w-32" data-input-number>
  <label class="label-text" for="number-input-mini">Quantity:</label>
  <div class="input items-center">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <input class="text-center" type="text" value="0" aria-label="Mini stacked buttons" data-input-number-input id="number-input-mini" />
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </div>
</div>
```

<!-- Booking -->

### Booking

Here's an example of a movie ticket booking number counter.

```html
<!-- Number of seat -->
<div class="input input-lg relative max-w-sm px-0" data-input-number>
  <span class="border-base-content/25 border-e ps-0">
    <button type="button" class="flex size-11.5 items-center justify-center" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
  </span>
  <input class="pb-2 text-center" type="text" value="0" aria-label="seat counter" data-input-number-input id="number-input-booking" />
  <div class="absolute start-1/2 bottom-0.5 flex -translate-x-1/2 items-center rtl:translate-x-1/2">
    <span class="icon-[tabler--ticket] text-base-content/80 me-2 size-4"></span>
    <span class="text-base-content/80 text-xs text-nowrap">Number of seat</span>
  </div>
  <span class="border-base-content/25 border-s pe-0">
    <button type="button" class="flex size-11.5 items-center justify-center" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>

<!-- Number of Bucket -->
<div class="input input-lg relative max-w-sm px-0" data-input-number>
  <span class="border-base-content/25 border-e ps-0">
    <button type="button" class="flex size-11.5 items-center justify-center" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
  </span>
  <input class="pb-2 text-center" id="number-input-bucket" type="text" value="0" aria-label="Bucket counter" data-input-number-input id="number-input-booking" />
  <div class="absolute start-1/2 bottom-0.5 flex -translate-x-1/2 items-center rtl:translate-x-1/2">
    <span class="icon-[tabler--brand-bitbucket] text-base-content/80 me-2 size-4"></span>
    <span class="text-base-content/80 text-xs text-nowrap">Number of Bucket</span>
  </div>
  <span class="border-base-content/25 border-s pe-0">
    <button type="button" class="flex size-11.5 items-center justify-center" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Step controls -->

### Step controls

Increase or decrease values in steps. This example uses a `":step"` value of `5`.

```html
<div class="input max-w-sm" data-input-number='{ "step": 5 }'>
  <input type="text" value="0" aria-label="Step control" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Min/Max value -->

### Min/Max value

You can control the minimum value with `":min"` and set the maximum value with `":max"`.

<!-- Maximum value -->

#### Maximum value

In the example below, the maximum number that can be selected is `15`.

```html
<div class="input max-w-sm" data-input-number='{ "max": 15 }'>
  <input type="text" value="1" aria-label="Maximum value input" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Negative value -->

#### Negative value

In the example below, the minimum number that can be selected is `-15`.

```html
<div class="input max-w-sm" data-input-number='{ "min": -15 }'>
  <input type="text" value="0" aria-label="Minimum value input" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>
```

<!-- Destroy/Reinitialize -->
### Destroy/Reinitialize
The `destroy` <a href="#destroy-method" class="link link-primary">method</a> is provided to facilitate the destruction of a input number.

```html
<div id="input-number-to-destroy" class="input max-w-sm" data-input-number>
  <input type="text" value="1" aria-label="Input number destroy" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>

<div class="mt-4 flex gap-3">
  <button class="btn btn-primary" id="destroy-btn">Destroy</button>
  <button class="btn btn-primary" id="reinit-btn" disabled>Reinitialize</button>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', () => {
    // Destroy and reinit variables
    const inputNumber = document.querySelector('#input-number-to-destroy')
    const destroyBtn = document.querySelector('#destroy-btn')
    const reinitBtn = document.querySelector('#reinit-btn')

    // Destroy usage
    destroyBtn.addEventListener('click', () => {
      const { element } = HSInputNumber.getInstance(inputNumber, true)

      element.destroy()

      destroyBtn.setAttribute('disabled', 'disabled')
      reinitBtn.removeAttribute('disabled')
    })

    // Reinit usage
    reinitBtn.addEventListener('click', () => {
      HSInputNumber.autoInit()

      reinitBtn.setAttribute('disabled', 'disabled')
      destroyBtn.removeAttribute('disabled')
    })
  })
</script>
```

<!-------------------- JavaScript behavior -------------------->

## JavaScript behavior

<!-- Options -->

### Options

> **Info:** FlyonUI is powered by <a href="https://preline.co/plugins/html/input-number.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

{{< table >}}
PARAMETERS|DESCRIPTION|OPTIONS|DEFAULT VALUE
<span class="text-nowrap">`data-input-number`</span>| <span class="text-pretty">Activate an Input Number by specifying on an element.</span>|`-`|`-`
`data-input-number-input`| Applied to the input element. |`-` | `-`
`data-input-number-increment`| Applied to the increment button. | `-` |`-`
`data-input-number-decrement`| Applied to the decrement button. | `-` |`-`
`:step`|Determines the step by which the value will increase or decrease. | number | `1`
`:min`| Defines the minimum value that can be entered. Setting it to `-Infinity` allows unrestricted negative values. | number /<br> "-Infinity" | `0`
`:max`|max Defines the maximum possible value.|number / null| `null`
{{< /table >}}

<!-- Methods -->

### Methods

The `HSInputNumber` object is contained within the global `window` object.

{{< table >}}

METHOD|DESCRIPTION
<span colspan="2" class="text-base-content font-semibold">PUBLIC METHODS</span>
`destroy()` | Destroys the instance, removes generated markup (if any), removes added classes and attributes.
<span colspan="2" class="text-base-content font-semibold">STATIC METHODS</span>
`HSInputNumber.getInstance(target, isInstance)`|<div>Returns the element associated to the <code>target</code>.<ul class="m-0"><li><code>target</code> should be a Node or string (valid selector).</li><li><code>isInstance</code> boolean. Returns the instance instead of Node if <code>true</code>.</li></ul></div>
{{< /table >}}

<p class="mt-5 mb-1.5 not-prose" id="destroy-method">Destroy instance.</p>

```js
const { element } = HSInputNumber.getInstance('#input-number-to-destroy', true);
const destroyBtn = document.querySelector('#destroy-btn');

destroyBtn.addEventListener('click', () => {
  element.destroy();
});
```

<!-- Events -->

### Events

{{< table >}}
METHOD| DESCRIPTION | RETURNING VALUE
`on:change`|Called when input value is changed.| Current value.

{{< /table >}}

<!-- Event usage -->

#### Event usage

Assign an ID to the `data-input-number` in the events. Increment the number and check the output in the console.

```html
<div id="input-number" class="input max-w-sm" data-input-number>
  <input type="text" value="1" aria-label="Number input" data-input-number-input />
  <span class="my-auto flex gap-3">
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Decrement button" data-input-number-decrement >
      <span class="icon-[tabler--minus] size-3.5 shrink-0"></span>
    </button>
    <button type="button" class="btn btn-primary btn-soft size-5.5 min-h-0 rounded-sm p-0" aria-label="Increment button" data-input-number-increment >
      <span class="icon-[tabler--plus] size-3.5 shrink-0"></span>
    </button>
  </span>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    const el = HSInputNumber.getInstance('#input-number')
  
    el.on('change', ({ inputValue }) => {
      console.log('Changed to:', inputValue)
    })
  })
</script>
```

<p class="mt-12 mb-1.5 not-prose">Open any accordion event example.</p>

```js
const el = HSInputNumber.getInstance('#input-number');

el.on('change', ({inputValue}) => {console.log('Changed to:', inputValue)});
```
