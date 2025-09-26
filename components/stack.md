# Stack

The Stack component is used to position elements on top of one another in a visually layered manner.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| stack | component | Stacks the child elements on top of each other. |
| stack-start | placement | Sets stacking direction to start. |
| stack-end | placement | Sets stacking direction to end. |
| stack-bottom-start | placement | Sets stacking direction to bottom-start. |
| stack-bottom-end | placement | Sets stacking direction to bottom-end. |
| stack-top | placement | Sets stacking direction to top. |
| stack-top-start | placement | Sets stacking direction to top-start. |
| stack-top-end | placement | Sets stacking direction to top-end. |
| stack-animated | placement | Adds animation to stack when hovered over. |


<!-------------------- Variants -------------------->

## Variants

<!--  Without stack  -->

### Without stack

The following example displays div's without stacking.

```html
<div>
  <div class="bg-primary text-primary-content grid h-20 w-32 place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid h-20 w-32 place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid h-20 w-32 place-content-center rounded-sm">3</div>
</div>
```

<!--  With stack  -->

### With stack

Wrap the stacked div's with a wrapper div using the component class `stack`.

```html
<div class="stack h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>  
</div>
```

<!-- Animated stack  -->

### Animated stack

Apply the modifier class stack-animated to enable animation on hover.

> **Info:** The `stack-animated modifier` class is also applicable to stacks with various positions.

```html
<div class="stack stack-bottom-start stack-animated h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-------------------- Positions -------------------->

## Positions

<!-- Bottom (default)  -->

### Bottom (default)

By default, the stacking direction is from the bottom.

```html
<div class="stack h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Bottom start  -->

### Bottom start

Apply the modifier class `stack-bottom-start` to set the stack direction to bottom-start.

```html
<div class="stack stack-bottom-start h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!--  Bottom end  -->

### Bottom end

Apply the modifier class `stack-bottom-end` to set the stack direction to bottom-end.

```html
<div class="stack stack-bottom-end h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Top  -->

### Top

Apply the modifier class `stack-top` to set the stack direction to top.

```html
<div class="stack stack-top h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Top start  -->

### Top start

Apply the modifier class `stack-top-start` to set the stack direction to top-start.

```html
<div class="stack stack-top-start h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Top end  -->

### Top end

Apply the modifier class `stack-top-end` to set the stack direction to stack-end.

```html
<div class="stack stack-top-end h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Start  -->

### Start

Apply the modifier class `stack-start` to set the stack direction to start.

```html
<div class="stack stack-start h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- End  -->

### End

Apply the modifier class `stack-end` to set the stack direction to end.

```html
<div class="stack stack-end h-20 w-32">
  <div class="bg-primary text-primary-content grid place-content-center rounded-sm">1</div>
  <div class="bg-success text-success-content grid place-content-center rounded-sm">2</div>
  <div class="bg-warning text-warning-content grid place-content-center rounded-sm">3</div>
</div>
```

<!-- Illustrations -->

## Illustrations

<!-- Stacked images  -->

### Stacked images

The example below demonstrates a stack with images.

```html
<div class="stack w-32">
  <img src="https://cdn.flyonui.com/fy-assets/components/card/image-1.png" alt="iphone" class="rounded-sm" />
  <img src="https://cdn.flyonui.com/fy-assets/components/card/image-2.png" alt="sydney" class="rounded-sm" />
  <img src="https://cdn.flyonui.com/fy-assets/components/card/image-3.png" alt="rome" class="rounded-sm" />
</div>
```

<!--  Stacked cards  -->

### Stacked cards

The example below demonstrates a stack with cards.

```html
<div class="stack w-32">
  <div class="card border-base-content border shadow-none">
    <div class="card-body text-center">
      <p>Card A</p>
    </div>
  </div>
  <div class="card border-base-content border shadow-none">
    <div class="card-body text-center">
      <p>Card B</p>
    </div>
  </div>
  <div class="card border-base-content border shadow-none">
    <div class="card-body text-center">
      <p>Card C</p>
    </div>
  </div>
</div>
```

<!--  notifications  -->

### Stacked notifications

The example below demonstrates a notifications stack.

```html
<div class="stack stack-animated">
  <div class="card bg-primary text-primary-content shadow-none">
    <div class="card-body">
      <h5 class="card-title text-primary-content">3 Notifications</h5>
      <p>You have 3 unread messages. Tap here to see.</p>
    </div>
  </div>
  <div class="card bg-info text-info-content shadow-none">
    <div class="card-body">
      <h5 class="card-title text-info-content">2 Notifications</h5>
      <p>You have 2 unread messages. Tap here to see.</p>
    </div>
  </div>
  <div class="card bg-secondary text-secbg-secondary-content shadow-none">
    <div class="card-body">
      <h5 class="card-title text-secbg-secondary-content">Notification 1</h5>
      <p>You have an unread message. Tap here to see.</p>
    </div>
  </div>
</div>
```
