# Status

The Status component is a compact icon designed to visually indicate the current state of an element, such as online, offline, or error.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| status | component | Status component |
| status-primary | color | Status with 'primary' color. |
| status-secondary | color | Status with 'secondary' color. |
| status-accent | color | Status with 'accent' color. |
| status-info | color | Status with 'info' color. |
| status-success | color | Status with 'success' color. |
| status-warning | color | Status with 'warning' color. |
| status-error | color | Status with 'error' color. |
| status-xs | size | Status with extra small size. |
| status-sm | size | Status with small size. |
| status-md | size | Status with medium (Default) size. |
| status-lg | size | Status with large size. |
| status-xl | size | Status with extra large size. |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic example of `status` component.

```html
<span class="status"></span>
```

<!-------------------- Size -------------------->

## Size

<!-- Status Sizes -->

### Status Sizes

Status sizes with `status-{xs|sm|md|lg|xl}` utility classes.

```html
<div aria-label="status" class="status status-xs"></div>
<div aria-label="status" class="status status-sm"></div>
<div aria-label="status" class="status status-md"></div>
<div aria-label="status" class="status status-lg"></div>
<div aria-label="status" class="status status-xl"></div>
```

<!-------------------- Color -------------------->

## Color

<!-- Semantic colors -->

### Semantic colors

Pre-configured color status designs.

```html
<div aria-label="status" class="status status-primary"></div>
<div aria-label="status" class="status status-secondary"></div>
<div aria-label="status" class="status status-accent"></div>
<div aria-label="info" class="status status-info"></div>
<div aria-label="success" class="status status-success"></div>
<div aria-label="warning" class="status status-warning"></div>
<div aria-label="error" class="status status-error"></div>
```

<!-------------------- Animation -------------------->

## Animation

<!-- Bounce Animation -->

### Bounce Animation

Use the `animate-bounce` utility to apply a bouncing animation to an element, creating a dynamic up-and-down motion. This effect is useful for drawing attention to interactive elements like buttons, notifications, or alerts.

```html
<div class="flex items-center gap-2">
  <div class="status status-info animate-bounce"></div>
  <span>Unread messages</span>
</div>
```

<!-- Ping Animation -->

### Ping Animation

Include the `animate-ping` utility to enable an element to scale and fade, resembling a radar ping or water ripple effect, which is beneficial for features like attention to the alert.

```html
<div class="flex items-center gap-2">
  <div class="inline-grid *:[grid-area:1/1]">
    <div class="status status-error animate-ping"></div>
    <div class="status status-error"></div>
  </div>
  <span>Server is down</span>
</div>
```

<!-- Pulse Animation -->

### Pulse Animation

Use the `animate-pulse` utility to make an element pulse, drawing attention to important statuses like alerts or maintenance.

```html
<div class="flex items-center gap-2">
  <div class="status status-warning animate-pulse"></div>
  <span>Under Maintenance</span>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Status with progress -->

### Status with progress

This example demonstrates how to integrate `status` with `progress` for better task visualization.

```html
<div class="progress mb-4 h-3">
  <div class="progress-bar progress-primary w-1/4 rounded-e-none"></div>
  <div class="progress-bar progress-success w-1/4 rounded-none"></div>
  <div class="progress-bar progress-error w-2/4 rounded-s-none"></div>
</div>
<div class="flex items-center gap-4 *:flex *:items-center *:gap-2">
  <div>
    <div aria-label="status" class="status status-primary"></div>
    <span class="text-primary">Initiated</span>
  </div>
  <div>
    <div aria-label="status" class="status status-success"></div>
    <span class="text-success">In Progress</span>
  </div>
  <div>
    <div aria-label="status" class="status status-error"></div>
    <span class="text-error">Completed</span>
  </div>
</div>
```
