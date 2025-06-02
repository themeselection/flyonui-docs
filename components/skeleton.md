# Skeleton

The skeleton component is utilized to display the loading state of a component.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| skeleton | component | Displays a markup's structure. |
| skeleton-animated | modifier | Displays skeleton with loading animation. |


<!-------------------- Variants -------------------->

## Variants

<!--  Default skeleton  -->

### Default skeleton

Apply the `skeleton` component class to any markup to showcase it's structure.

```html
<div class="skeleton h-32 w-32"></div>
```

<!--  Animated skeleton  -->

### Animated skeleton

Apply the `skeleton-animated` modifier class to any markup to showcase it's structure with loading animation.

```html
<div class="skeleton skeleton-animated h-32 w-32"></div>
```

<!--  Active skeleton  -->

### Active skeleton

Add the `animate-pulse` animation class to any markup to display its structure with an active animation. For additional options, refer to the TailwindCSS <a href="https://tailwindcss.com/docs/animation" target="_blank" class="link link-primary">animation</a> documentation.

```html
<div class="skeleton h-32 w-32 animate-pulse"></div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!--  Circle with content  -->

### Circle with content

Utilize the provided example to present a skeleton featuring a circular shape and content.

```html
<div class="flex w-52 flex-col gap-4">
  <div class="flex items-center gap-4">
    <div class="skeleton h-16 w-16 shrink-0 rounded-full"></div>
    <div class="flex flex-col gap-4">
      <div class="skeleton h-4 w-20"></div>
      <div class="skeleton h-4 w-28"></div>
    </div>
  </div>
  <div class="skeleton h-32 w-full"></div>
</div>
```

<!--  Rectangle with content  -->

### Rectangle with content

Utilize the provided example to present a skeleton featuring a Rectangular shape and content with loading animation.

```html
<div class="flex w-52 flex-col gap-4">
  <div class="skeleton skeleton-animated h-32 w-full"></div>
  <div class="skeleton skeleton-animated h-4 w-28"></div>
  <div class="skeleton skeleton-animated h-4 w-full"></div>
  <div class="skeleton skeleton-animated h-4 w-full"></div>
</div>
```
