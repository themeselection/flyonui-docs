# Alert

Alerts are designed to notify users about important events, updates, or changes that require their attention.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| alert | component | Container element |
| alert-soft | style | Soft color alert with border |
| alert-outline | style | Alert with border |
| alert-primary | color | Alert with 'primary' color |
| alert-secondary | color | Alert with 'secondary' color |
| alert-info | color | Alert with 'info' color |
| alert-success | color | Alert with 'success' color |
| alert-warning | color | Alert with 'warning' color |
| alert-error | color | Alert with 'error' color |


<!-------------------- Variants -------------------->

## Variants

<!-- Solid alerts -->

### Solid alerts

The standard format of solid-colored avatars, accompanied by the component class `alert` and modifier class <br />
`alert-{semantic-color}`.

```html
<div class="alert" role="alert">
  A quick alert conveying key information or prompting action within a system.
</div>
<div class="alert alert-primary" role="alert">Welcome to our platform! Explore our latest features and updates.</div>
<div class="alert alert-info" role="alert">Stay tuned for our upcoming events and announcements.</div>
<div class="alert alert-success" role="alert">Your transaction was successful. Thank you for choosing our service!</div>
<div class="alert alert-warning" role="alert">
  Attention! Your account security may be at risk. Enable two-factor authentication now.
</div>
<div class="alert alert-error" role="alert">Oops! It seems there was an unexpected error. Please try again later.</div>
```

<!-- Soft alerts -->

### Soft alerts

The standard format of soft-colored avatars, accompanied by the component class `alert` , `alert-soft` and modifier class `alert-{semantic-color}`.

```html
<div class="alert alert-soft" role="alert">
  A quick alert conveying key information or prompting action within a system.
</div>
<div class="alert alert-soft alert-primary" role="alert">
  Welcome to our platform! Explore our latest features and updates.
</div>
<div class="alert alert-soft alert-info" role="alert">Stay tuned for our upcoming events and announcements.</div>
<div class="alert alert-soft alert-success" role="alert">
  Your transaction was successful. Thank you for choosing our service!
</div>
<div class="alert alert-soft alert-warning" role="alert">
  Attention! Your account security may be at risk. Enable two-factor authentication now.
</div>
<div class="alert alert-soft alert-error" role="alert">
  Oops! It seems there was an unexpected error. Please try again later.
</div>
```

<!-- Outline alerts -->

### Outline alerts

The standard format of outline-colored avatars, accompanied by the component class `alert` , `alert-outline` and modifier class `alert-{semantic-color}`.

```html
<div class="alert alert-outline" role="alert">
  A quick alert conveying key information or prompting action within a system.
</div>
<div class="alert alert-outline alert-primary" role="alert">
  Welcome to our platform! Explore our latest features and updates.
</div>
<div class="alert alert-outline alert-info" role="alert">Stay tuned for our upcoming events and announcements.</div>
<div class="alert alert-outline alert-success" role="alert">
  Your transaction was successful. Thank you for choosing our service!
</div>
<div class="alert alert-outline alert-warning" role="alert">
  Attention! Your account security may be at risk. Enable two-factor authentication now.
</div>
<div class="alert alert-outline alert-error" role="alert">
  Oops! It seems there was an unexpected error. Please try again later.
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Dashed alerts -->

### Dashed alerts

You can achieve this style by combining the `border-dashed` utility class with the `alert-outline` modifier class.

```html
<div class="alert alert-outline border-dashed" role="alert">
  A quick alert conveying key information or prompting action within a system.
</div>
<div class="alert alert-outline border-dashed alert-primary" role="alert">
  Welcome to our platform! Explore our latest features and updates.
</div>
<div class="alert alert-outline border-dashed alert-info" role="alert">Stay tuned for our upcoming events and announcements.</div>
<div class="alert alert-outline border-dashed alert-success" role="alert">
  Your transaction was successful. Thank you for choosing our service!
</div>
<div class="alert alert-outline border-dashed alert-warning" role="alert">
  Attention! Your account security may be at risk. Enable two-factor authentication now.
</div>
<div class="alert alert-outline border-dashed alert-error" role="alert">
  Oops! It seems there was an unexpected error. Please try again later.
</div>
```

<!-- Alerts with icon -->

### Alerts with icon

Add a descriptive icon to complement the message within the alert component, as illustrated in the example below.

```html
<div class="alert alert-warning flex items-center gap-4" role="alert">
  <span class="icon-[tabler--alert-triangle] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Warning alert:</span> Stay informed about the latest updates and upcoming events.</p>
</div>

<div class="alert alert-success flex items-center gap-4" role="alert">
  <span class="icon-[tabler--circle-check] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Success alert:</span> Explore our recent achievements and upcoming events.
  </p>
</div>

<div class="alert alert-soft alert-warning flex items-center gap-4" role="alert">
  <span class="icon-[tabler--alert-triangle] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Warning alert:</span> Take note of important updates and upcoming events.
  </p>
</div>

<div class="alert alert-soft alert-success flex items-center gap-4" role="alert">
  <span class="icon-[tabler--circle-check] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Success alert:</span> Celebrate our successes and stay informed about upcoming events.
  </p>
</div>

<div class="alert alert-outline alert-warning flex items-center gap-4" role="alert">
  <span class="icon-[tabler--alert-triangle] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Warning alert:</span> Pay attention to warnings and stay updated about upcoming events.
  </p>
</div>

<div class="alert alert-outline alert-success flex items-center gap-4" role="alert">
  <span class="icon-[tabler--circle-check] shrink-0 size-6"></span>
  <p><span class="text-lg font-semibold">Success alert:</span> Be aware of important notices and upcoming events.
  </p>
</div>
```

<!-- Descriptive alert -->

### Descriptive alert

Alerts may include supplementary HTML elements such as headers, paragraphs, and icons.

```html
<div class="alert alert-soft alert-primary flex items-start gap-4">
  <span class="icon-[tabler--check] shrink-0 size-6"></span>
  <div class="flex flex-col gap-1">
    <h5 class="text-lg font-semibold">Server maintenance in progress</h5>
    <p>Our servers are currently undergoing maintenance. We apologize for any inconvenience caused and appreciate your patience.
    </p>
  </div>
</div>
```

<!-- Alert with list -->

### Alert with list

Similarly you can use lists.

```html
<div class="alert alert-soft alert-primary flex items-start gap-4">
  <span class="icon-[tabler--info-circle] shrink-0 size-6"></span>
  <div class="flex flex-col gap-1">
    <h5 class="text-lg font-semibold">Please ensure that your password meets the following requirements:</h5>
    <ul class="mt-1.5 list-inside list-disc">
      <li>Contains a minimum of 10 characters and a maximum of 100 characters.</li>
      <li>Includes at least one lowercase character.</li>
      <li>Incorporates at least one special character such as !, @, #, or ?.</li>
    </ul>
  </div>
</div>
```

<!-- Alert with action -->

### Alert with action

The action alert delivers vital information to users and encourages them to take defined actions. It commonly comprises a message, a link for additional details, and interactive buttons for user engagement.

```html
<div class="alert alert-soft alert-primary" role="alert">
  Please read the <a href="#" class="link link-primary font-semibold">policy</a>. These can be configured in Settings.
  <div class="mt-4 flex gap-2">
    <button type="button" class="btn btn-primary btn-sm">Ok</button>
    <button type="button" class="btn btn-outline btn-secondary btn-sm">Cancel</button>
  </div>
</div>
```

<!-- Responsive alert -->

### Responsive alert

This alert example maintains a horizontal layout on larger screens while adapting to a vertical layout on mobile devices.

```html
<div class="alert alert-soft alert-primary flex items-start max-sm:flex-col max-sm:items-center gap-4">
  <span class="icon-[tabler--check] size-6 shrink-0"></span>
  <div class="flex flex-col grow gap-1 max-sm:items-center">
    <h5 class="text-lg font-semibold">Server maintenance in progress</h5>
    <p>Our servers are currently undergoing maintenance. We apologize for any inconvenience caused and appreciate your patience.</p>
  </div>
  <div class="flex gap-2">
    <button type="button" class="btn btn-primary btn-sm">Agree</button>
    <button type="button" class="btn btn-outline btn-secondary btn-sm">Cancel</button>
  </div>
</div>
```

{{< requires-js >}}

<!-- Dismissible alert -->

### Dismissible alert

Utilize the `data-remove-element` attribute to specify the connected ID for alert removal. Customize the removal animation by incorporating the `removing:` modifier, as illustrated below.

> **Info:** Refer [Remove Element](components/remove-element/) plugin for more details.

```html
<div class="alert alert-soft alert-primary removing:translate-x-5 removing:opacity-0 flex items-center gap-4 transition duration-300 ease-in-out" role="alert" id="dismiss-alert1">
  Dive into our platform to discover exciting new features and updates.
  <button class="ms-auto cursor-pointer leading-none" data-remove-element="#dismiss-alert1" aria-label="Close Button">
    <span class="icon-[tabler--x] size-5"></span>
  </button>
</div>
```
