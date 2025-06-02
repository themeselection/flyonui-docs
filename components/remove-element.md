# Remove element

Easily remove elements with just a single click, streamlining your workflow and enhancing user experience.

> **Info:** Remove element components are adopted from Preline UI components using <a href="https://preline.co/plugins.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

<!-- Class Table -->

| Class | Type | Description |
| --- | --- | --- |
| removing: | variant | When the removal process starts, it applies a specified class. |


<!-------------------- Default -------------------->

## Default

<!-- Basic example -->

### Basic example

Include the `data-remove-element` attribute in the close button element and set its value to `#id` to specify the element to be removed.
Customize the removal animation by incorporating the `removing:` modifier, as illustrated below.

```html
<div class="card removing:opacity-0 removing:translate-x-5 bg-primary/20 text-primary max-w-sm transition duration-300 ease-in-out" id="card-dismiss" >
  <div class="card-header text-base-content/80 flex justify-between items-center">
    <span class="card-title text-primary">Remove card</span>
    <div class="card-actions">
      <button class="cursor-pointer leading-none" data-remove-element="#card-dismiss" aria-label="Close Button" >
        <span class="icon-[tabler--x] size-5 text-primary"></span>
      </button>
    </div>
  </div>
  <div class="card-body">
    <p>With a single click on the close button, this card will be effortlessly removed.</p>
  </div>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Chip -->

### Badge

Below example demonstrates use of `remove-element` in badges.

```html
<span class="badge badge-soft badge-lg badge-primary removing:translate-x-5 removing:opacity-0 transition duration-300 ease-in-out" id="badge-chip" >
  Badge
  <button class="icon-[tabler--circle-x-filled] size-5 min-h-0 cursor-pointer px-0 opacity-70" data-remove-element="#badge-chip" aria-label="Close Button" ></button>
</span>
```

<!-- Alerts -->

### Alerts

Below example demonstrates use of `remove-element` in alerts.

```html
<div class="alert alert-soft alert-primary removing:translate-x-5 removing:opacity-0 flex items-center gap-4 transition duration-300 ease-in-out" role="alert" id="dismiss-alert" >
  Dive into our platform to discover exciting new features and updates.
  <button class="ms-auto cursor-pointer leading-none" data-remove-element="#dismiss-alert" aria-label="Close Button" >
    <span class="icon-[tabler--x] size-5"></span>
  </button>
</div>
```

<!-- Destroy/Reinitialize -->
### Destroy/Reinitialize
The `destroy` <a href="#destroy-method" class="link link-primary">method</a> is provided to facilitate the destruction of a remove element.

```html
<div class="card removing:opacity-0 removing:translate-x-5 bg-primary/20 text-primary max-w-sm transition duration-300 ease-in-out" id="remove-element-to-destroy" >
  <div class="card-header text-base-content/80 flex justify-between items-center">
    <span class="card-title text-primary">Remove card</span>
    <div class="card-actions">
      <button class="cursor-pointer leading-none" data-remove-element="#remove-element-to-destroy" aria-label="Close Button" >
        <span class="icon-[tabler--x] size-5 text-primary"></span>
      </button>
    </div>
  </div>
  <div class="card-body">
    <p>With a single click on the close button, this card will be effortlessly removed.</p>
  </div>
</div>

<div class="mt-4 flex gap-3">
  <button class="btn btn-primary" id="destroy-btn">Destroy</button>
  <button class="btn btn-primary" id="reinit-btn" disabled>Reinitialize</button>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', () => {
    // Destroy and reinit variables
    const removeElement = document.querySelectorAll('#remove-element-to-destroy [data-remove-element]')
    const destroyBtn = document.querySelector('#destroy-btn')
    const reinitBtn = document.querySelector('#reinit-btn')

    // Destroy usage
    destroyBtn.addEventListener('click', () => {
      removeElement.forEach(el => {
        const { element } = HSRemoveElement.getInstance(el, true)

        element.destroy()
      })

      destroyBtn.setAttribute('disabled', 'disabled')
      reinitBtn.removeAttribute('disabled')
    })

    // Reinit usage
    reinitBtn.addEventListener('click', () => {
      HSRemoveElement.autoInit()

      reinitBtn.setAttribute('disabled', 'disabled')
      destroyBtn.removeAttribute('disabled')
    })
  })
</script>
```

<!-------------------- Options usage -------------------->

## Options usage

<!-- Using data attribute -->

### Using data attribute

In the `data-remove-element-options` attribute, assign an object as its value.

Within this object, define the `removeTargetAnimationClass` key as a Tailwind CSS class, which will be applied during the removal process.By default, this value is derived from the modifier class `removing:`, but it can also be specified using this data attribute option.

```html
<div class="card removing:opacity-0 bg-primary/20 text-primary max-w-sm transition duration-300 ease-in-out" id="card-dismiss-2" >
  <div class="card-header text-base-content/80 flex justify-between items-center">
    <span class="card-title text-primary">Remove card</span>
    <div class="card-actions">
      <button class="cursor-pointer leading-none" data-remove-element="#card-dismiss-2" data-remove-element-options='{"removeTargetAnimationClass":"translate-x-5"}' aria-label="Close Button" >
        <span class="icon-[tabler--x] size-5 text-primary"></span>
      </button>
    </div>
  </div>
  <div class="card-body">
    <p>With a single click on the close button, this card will be effortlessly removed.</p>
  </div>
</div>
```

<!-------------------- JavaScript behavior -------------------->

## JavaScript behavior

> **Info:** FlyonUI is powered by <a href="https://preline.co/plugins/html/remove-element.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

<!--  Options  -->

### Options

{{< table >}}

PARAMETERS|DESCRIPTION|OPTIONS|DEFAULT VALUE
`data-remove-element`| The element to be removed. This must be a valid selector.|`-`|`null`
`data-remove-element-options`| Option that can be added via the data attribute.| `-` | `-`
`:removeTargetAnimationClass`| Some valid TailwindCSS class.| string | `removing`
{{< /table >}}

<!-- Methods -->

### Methods

The `HSRemoveElement` object is contained within the global `window` object.

{{< table >}}
METHOD|DESCRIPTION
<span colspan="2" class="text-base-content font-semibold">PUBLIC METHODS</span>
`destroy()`| Destroys the instance, removes generated markup (if any), removes added classes and attributes.
<span colspan="2" class="text-base-content font-semibold">STATIC METHODS</span>
`HSRemoveElement.getInstance(target, isInstance)`|<div>Returns the element associated to the <code>target</code>.<ul class="m-0"><li><code>target</code> should be a Node or string (valid selector).</li><li><code>isInstance</code> boolean. Returns the instance instead of Node if <code>true</code>.</li></ul></div>
{{< /table >}}

<p id="destroy-method" class="mt-10 mb-1.5 not-prose">Destroy the instance if the `Id` is added to the `data-remove-element` attribute, or use it as shown in the example above.</p>

```js
const { element } = HSRemoveElement.getInstance('#remove-element', true);
const destroyBtn = document.querySelector('#destroy-btn');

destroyBtn.addEventListener('click', () => {
  element.destroy();
});
```
