# Radial progress

Radial progress can visually represent either the completion of a task or the elapsed passage of time.

<!-- Class Table -->

| Class | Type | Description |
| --- | --- | --- |
| radial-progress | component | Base class for radial progress component. |


> **Info:** <div>
>   <p>The radial progress component requires the <code class="text-sm">--value</code> CSS variable to define its progress percentage.</p>
>   <p>To adjust its size, use the <code class="text-sm">--size</code> CSS variable, which defaults to 5rem.</p>
>   <p>To modify the thickness of the progress ring, use the <code class="text-sm">--thickness</code> CSS variable, which is set to 10% of the size by default.</p>
> </div>


> **Info:** <div>
>   <p> For Radial progress we need to use a <code class="text-sm">div</code> instead of the <code class="text-sm">progress</code> tag because browsers can’t show text inside <code class="text-sm">progress</code> tag, and Firefox doesn’t render pseudo-elements inside <code class="text-sm">progress</code> tag at all.</p>
>   <p class="mt-1.5">Adding <code class="text-sm">role="progressbar"</code> makes it accessible to screen readers as well.</p>
> </div>


<!-------------------- Variants -------------------->

## Variants

<!-- Default -->

### Default

Utilize the `radial-progress` component class and adjust the progress value by setting the CSS variable `--value:*` in
the style attribute of the radial progress component, where `*` represents a numerical value.

```html
<div class="radial-progress" style="--value:75;" role="progressbar" aria-label="Radial Progress"></div>
```

<!-- With values -->

### With values

Embed a value in the radial progress component markup to visualize the progress accordingly.

```html
<div class="radial-progress" style="--value:0;" role="progressbar" aria-label="0% Radial Progressbar">0%</div>
<div class="radial-progress" style="--value:20;" role="progressbar" aria-label="20% Radial Progressbar">20%</div>
<div class="radial-progress" style="--value:60;" role="progressbar" aria-label="60% Radial Progressbar">60%</div>
<div class="radial-progress" style="--value:80;" role="progressbar" aria-label="80% Radial Progressbar">80%</div>
<div class="radial-progress" style="--value:100;" role="progressbar" aria-label="100% Radial Progressbar">100%</div>
```

<!-- With text  -->

### With text

Embed a value & text in the radial progress component markup to visualize the radial progress with text.

```html
<div class="radial-progress" style="--value:60;" role="progressbar" aria-label="60% Radial Progressbar">
  <div class="mx-auto">60%</div>
  <span class="text-secondary text-xs">Loss</span>
</div>
<div class="radial-progress" style="--value:80;" role="progressbar" aria-label="80% Radial Progressbar">
  <div class="mx-auto">80%</div>
  <span class="text-secondary text-xs">Profit</span>
</div>
```

<!-- Colors -->

## Colors

<!-- Semantic -->

### Semantic

Apply the text utility class `text-{semantic-color}` to the radial progress to style it with semantic colors.

```html
<div class="radial-progress text-neutral" style="--value:70;" role="progressbar" aria-label="Neutral Radial Progressbar">70%</div>
<div class="radial-progress text-primary" style="--value:70;" role="progressbar" aria-label="Primary Radial Progressbar">70%</div>
<div class="radial-progress text-secondary" style="--value:70;" role="progressbar" aria-label="Secondary Radial Progressbar">70%</div>
<div class="radial-progress text-accent" style="--value:70;" role="progressbar" aria-label="Accent Radial Progressbar">70%</div>
<div class="radial-progress text-info" style="--value:70;" role="progressbar" aria-label="Info Radial Progressbar">70%</div>
<div class="radial-progress text-success" style="--value:70;" role="progressbar" aria-label="Success Radial Progressbar">70%</div>
<div class="radial-progress text-warning" style="--value:70;" role="progressbar" aria-label="Warning Radial Progressbar">70%</div>
<div class="radial-progress text-error" style="--value:70;" role="progressbar" aria-label="Error Radial Progressbar">70%</div>
```

<!-- With background -->

### With background

Utilize the provided examples to implement radial progress with semantic background colors.

```html
<div class="radial-progress bg-neutral text-neutral-content border-neutral border-4" style="--value:70;" role="progressbar" aria-label="Neutral Radial Progressbar">70%</div>
<div class="radial-progress bg-primary text-primary-content border-primary border-4" style="--value:70;" role="progressbar" aria-label="Primary Radial Progressbar">70%</div>
<div class="radial-progress bg-secondary text-secondary-content border-secondary border-4"style="--value:70;"role="progressbar" aria-label="Secondary Radial Progressbar">70%</div>
<div class="radial-progress bg-accent text-accent-content border-accent border-4" style="--value:70;" role="progressbar" aria-label="Accent Radial Progressbar">70%</div>
<div class="radial-progress bg-info text-info-content border-info border-4" style="--value:70;" role="progressbar" aria-label="Info Radial Progressbar">70%</div>
<div class="radial-progress bg-success text-success-content border-success border-4" style="--value:70;" role="progressbar" aria-label="Success Radial Progressbar">70%</div>
<div class="radial-progress bg-warning text-warning-content border-warning border-4" style="--value:70;" role="progressbar" aria-label="Warning Radial Progressbar">70%</div>
<div class="radial-progress bg-error text-error-content border-error border-4" style="--value:70;" role="progressbar" aria-label="Error Radial Progressbar">70%</div>
```

<!-- With soft background -->

### With soft background

Utilize the provided examples to implement radial progress with soft semantic background colors.

```html
<div class="radial-progress bg-neutral/10 text-neutral border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Neutral Radial Progressbar">70%</div>
<div class="radial-progress bg-primary/10 text-primary border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Primary Radial Progressbar">70%</div>
<div class="radial-progress bg-secondary/10 text-secondary border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Secondary Radial Progressbar">70%</div>
<div class="radial-progress bg-accent/10 text-accent border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Accent Radial Progressbar">70%</div>
<div class="radial-progress bg-info/10 text-info border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Info Radial Progressbar">70%</div>
<div class="radial-progress bg-success/10 text-success border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Success Radial Progressbar">70%</div>
<div class="radial-progress bg-warning/10 text-warning border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Warning Radial Progressbar">70%</div>
<div class="radial-progress bg-error/10 text-error border-4 border-transparent" style="--value:70;" role="progressbar" aria-label="Error Radial Progressbar">70%</div>
```

<!-------------------- Sizes -------------------->

## Sizes

<!-- Custom size & thickness -->

### Custom size & thickness

Modify the size and thickness of the progress by defining the CSS variables `--size:*` and `--thickness:*` within the style attribute of the radial progress component, where `*` denotes a numerical value along with the unit.

```html
<div class="radial-progress" style="--value:70; --size:12rem; --thickness: 2px;" role="progressbar" aria-label="Radial Progressbar">70%</div>
<div class="radial-progress" style="--value:70; --size:12rem; --thickness: 2rem;" role="progressbar" aria-label="Radial Progressbar">70%</div>
<div class="radial-progress bg-primary/10 text-primary border-4 border-transparent" style="--value:70; --size:12rem; --thickness: 1rem;" role="progressbar" aria-label="Radial Progressbar">70%</div>
```
