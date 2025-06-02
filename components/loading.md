# Loading

The loading animation visually indicates that a process is currently in progress.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| loading | component | Base class for loading component. |
| loading-spinner | style | Shows the spinner animation. |
| loading-dots | style | Shows the dots animation. |
| loading-ring | style | Shows the ring animation. |
| loading-ball | style | Shows the ball animation. |
| loading-bars | style | Shows the bars animation. |
| loading-infinity | style | Shows the infinity animation. |
| loading-xs | size | Makes the loading component extra small. |
| loading-sm | size | Makes the loading component small. |
| loading-md | size | Makes the loading component medium(default). |
| loading-lg | size | Makes the loading component large. |
| loading-xl | size | Makes the loading component extra-large. |


<!-------------------- Variants -------------------->

## Variants

<!-- Loading spinner -->

### Loading spinner

The standard format for loading is component class `loading`, accompanied by modifier class `loading-spinner` to show the
spinner animation. The size of the spinner can be adjusted using the responsive classes `loading-{size}` where `{size}`
can be `xs`, `sm`, `md`, `lg`  or `xl`.

```html
<span class="loading loading-spinner loading-xs"></span>
<span class="loading loading-spinner loading-sm"></span>
<span class="loading loading-spinner"></span>
<span class="loading loading-spinner loading-lg"></span>
<span class="loading loading-spinner loading-xl"></span>
```

<!-- Loading dots -->

### Loading dots

Use the modifier class `loading-dots` for loading with dots animation.

```html
<span class="loading loading-dots loading-xs"></span>
<span class="loading loading-dots loading-sm"></span>
<span class="loading loading-dots"></span>
<span class="loading loading-dots loading-lg"></span>
<span class="loading loading-dots loading-xl"></span>
```

<!-- Loading rings -->

### Loading rings

Use the modifier class `loading-ring` for loading with growing rings animation.

```html
<span class="loading loading-ring loading-xs"></span>
<span class="loading loading-ring loading-sm"></span>
<span class="loading loading-ring"></span>
<span class="loading loading-ring loading-lg"></span>
<span class="loading loading-ring loading-xl"></span>
```

<!-- Loading ball -->

### Loading ball

Use the modifier class `loading-ball` for loading with jumping balls animation.

```html
<span class="loading loading-ball loading-xs"></span>
<span class="loading loading-ball loading-sm"></span>
<span class="loading loading-ball"></span>
<span class="loading loading-ball loading-lg"></span>
<span class="loading loading-ball loading-xl"></span>
```

<!-- Loading bars -->

### Loading bars

Use the modifier class `loading-bars` for loading with bars animation.

```html
<span class="loading loading-bars loading-xs"></span>
<span class="loading loading-bars loading-sm"></span>
<span class="loading loading-bars"></span>
<span class="loading loading-bars loading-lg"></span>
<span class="loading loading-bars loading-xl"></span>
```

<!-- Loading infinity -->

### Loading infinity

Use the modifier class `loading-infinity` for loading with infinity animation.

```html
<span class="loading loading-infinity loading-xs"></span>
<span class="loading loading-infinity loading-sm"></span>
<span class="loading loading-infinity"></span>
<span class="loading loading-infinity loading-lg"></span>
<span class="loading loading-infinity loading-xl"></span>
```

<!-------------------- Colors -------------------->

## Colors

<!-- Colored spinners -->

### Colored spinners

Utilize the text utility class `text-{semantic-color}` to create loading animations with different colors, each corresponding to specific modifiers.

```html
<span class="loading loading-spinner text-primary"></span>
<span class="loading loading-spinner text-secondary"></span>
<span class="loading loading-spinner text-accent"></span>
<span class="loading loading-spinner text-neutral"></span>
<span class="loading loading-spinner text-info"></span>
<span class="loading loading-spinner text-success"></span>
<span class="loading loading-spinner text-warning"></span>
<span class="loading loading-spinner text-error"></span>
```

<!-- Illustrations -->

## Illustrations

<!-- Within buttons -->

### Within buttons

Below are the examples illustrating the integration of loading animations within buttons.

```html
<button class="btn btn-primary btn-square btn-disabled" aria-label="Loading Button">
  <span class="loading loading-spinner loading-sm"></span>
</button>
<button class="btn btn-primary btn-disabled">
  <span class="loading loading-spinner loading-sm"></span>
<span>Loading...</span>
</button>
<button class="btn btn-success btn-square btn-disabled" aria-label="Loading Button">
  <span class="loading loading-ring loading-sm"></span>
</button>
<button class="btn btn-success btn-disabled">
  <span>Ping</span>
<span class="loading loading-ring loading-sm"></span>
</button>
```

<!-- Within alerts -->

### Within alerts

Below are the examples illustrating the integration of loading animations within alerts.

```html
<div class="alert alert-primary border-0 flex items-center gap-4" role="alert">
  <span class="icon-[tabler--alert-triangle] size-5"></span>
  <p> <strong>Primary alert:</strong> Welcome to our platform! Explore our latest features and updates. </p>
  <div class="bg-base-100/50 absolute rounded-box start-0 top-0 size-full"></div>
  <div class="absolute start-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 transform">
    <span class="loading loading-spinner"></span>
  </div>
</div>

<div class="alert alert-success border-0 flex items-center gap-4" role="alert">
  <span class="icon-[tabler--circle-check] size-5"></span>
  <p> <strong>Success alert:</strong> Explore our recent achievements and upcoming events. </p>
  <div class="bg-base-100/50 absolute rounded-box start-0 top-0 size-full"></div>
  <div class="absolute start-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 transform">
    <span class="loading loading-spinner"></span>
  </div>
</div>
```

<!-- Within cards -->

### Within cards

Below is the example illustrating the integration of loading animations within cards.

```html
<div class="card group max-w-sm hover:shadow">
  <figure>
    <img src="https://cdn.flyonui.com/fy-assets/components/carousel/image-7.png" alt="Album" class="transition-transform duration-500 group-hover:scale-105" />
  </figure>
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p> This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer. </p>
  </div>
  <div class="card-footer">
    <small class="text-base-content/50">Last updated 3 mins ago</small>
  </div>
  <div class="bg-base-100/50 absolute start-0 top-0 size-full"></div>
  <div class="absolute start-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 transform">
    <span class="loading loading-spinner loading-lg text-primary"></span>
  </div>
</div>
```
