# Range

A range slider is used to modify a value by sliding a handle along a track, allowing for precise adjustments.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| range | component | Range input |
| range-primary | color | Adds 'primary' to range |
| range-secondary | color | Adds 'secondary' to range |
| range-accent | color | Adds 'accent' to range |
| range-info | color | Adds 'info' to range |
| range-success | color | Adds 'success' to range |
| range-warning | color | Adds 'warning' to range |
| range-error | color | Adds 'error' to range |
| range-xs | size | Extra small range |
| range-sm | size | Small range |
| range-md | size | Medium (Default) range |
| range-lg | size | Large range |
| range-xl | size | Extra Large range |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic input `range` example.

```html
<input type="range" class="range" aria-label="range" />
```

<!-------------------- Size -------------------->

## Size

<!-- Range sizes -->

### Range sizes

The Range inputs are stacked in three sizes:extra small `xs`, small `sm`, default, and large `lg`.

```html
<input type="range" class="range range-xs" aria-label="range" />
<input type="range" class="range range-sm" aria-label="range" />
<input type="range" class="range" aria-label="range" />
<input type="range" class="range range-lg" aria-label="range" />
<input type="range" class="range range-xl" aria-label="range" />
```

<!-------------------- Color  -------------------->

## Color

<!-- Semantic colors -->

### Semantic colors

The standard format for range is accompanied by the component class `range` and modifier class `range-{semantic-color}`.

```html
<input type="range" class="range" aria-label="range" />
<input type="range" class="range range-primary" aria-label="primary range" />
<input type="range" class="range range-secondary" aria-label="secondary range" />
<input type="range" class="range range-info" aria-label="info range" />
<input type="range" class="range range-success" aria-label="success range" />
<input type="range" class="range range-warning" aria-label="warning range" />
<input type="range" class="range range-error" aria-label="error range" />
```

<!-- Custom color -->

### Custom color

Utilize `[--range-color:]` to incorporate your custom color.

```html
<input type="range" class="range [--range-color:teal]" aria-label="custom range" />
```

<!-------------------- Illustration -------------------->

## Illustrations

<!-- Disabled -->

### Disabled

Apply the `disabled` boolean attribute to a range input to disable pointer events and prevent focusing.

```html
<input type="range" class="range" aria-label="disabled range" disabled />
```

<!-- Min and max -->

### Min and max

Range inputs inherently have default values for `min` and `max` - 0 and 100, respectively. You can customize these values using the `min` and `max` attributes.

```html
<input type="range" class="range" min="0" max="100" value="40" aria-label="range">
```

<!-- Steps -->

### Steps

The `step` attribute specifies the interval between legal numbers in an `<input>` element.

```html
<input type="range" min="0" max="100" value="25" class="range" step="25" aria-label="range" />

<div class="w-full flex justify-between text-xs px-2">
  <span>|</span>
  <span>|</span>
  <span>|</span>
  <span>|</span>
  <span>|</span>
</div>
```
