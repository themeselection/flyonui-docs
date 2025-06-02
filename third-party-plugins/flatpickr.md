# Flatpickr (Datepicker)

Flatpickr is a lightweight JavaScript library for easy date and time picking, offering sleek design and extensive customization options for web applications.

<!-------------------- Getting started -------------------->

## Getting started

<!-- Setup -->

### Setup

Below are the steps to seamlessly integrate <a href="https://flatpickr.js.org/" target="_blank" class="link link-primary">Flatpickr</a> JS into your project.

<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical mb-12 w-full ps-0">
  <!-- Installation -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        1
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Installation</div>
      <p> Install <code>flatpickr</code> using npm:</p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}npm i flatpickr{{< /code-highlight >}}
    </div>
    <hr class="!w-0.5 rounded-none border-transparent" />
  </li>
  
  <!-- Include JS and CSS -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        2
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Include Flatpickr JavaScript and CSS</div>
      <p>Include the necessary CSS and JavaScript files in the following locations:</p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="html" >}}
<head>
  <link rel="stylesheet" href="../path/to/flatpickr/dist/flatpickr.css" />
</head>
<body>
  <script src="../path/to/flatpickr/flatpickr.js"></script>
</body>
{{< /code-highlight >}}
      <p class="!mt-4">
        <strong>Note:</strong>  A CDN link won't work here because we need to modify the default Vendor CSS to fit FlyonUI's design.
      </p>
    </div>
    <hr class="!w-0.5 rounded-none border-transparent" />
  </li>
  
  <!-- Tailwind Configuration -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        3
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Update Tailwind Configuration</div>
      <p>Update your <code>tailwind.css</code> file to incorporate the path for the FlyonUI Flatpickr override CSS.</p>
      {{< code-highlight addClass="!mb-0 mt-2 max-h-96 highlight-top-rounded-none" lang="css" >}}@import "flyonui/src/vendor/flatpickr.css";{{< /code-highlight >}}
    </div>
    <hr class="!w-0.5 rounded-none border-transparent" />
  </li>
  
  <!-- Basic Usage -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        4
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Basic Usage</div>
      <p>The following are valid ways to create a Flatpickr instance:</p>
      {{< code-highlight addClass="!mb-0 mt-2" lang="js" >}}// If using Flatpickr in a framework, it's recommended to pass the element directly
flatpickr(element, {});

// Alternatively, selectors are supported
flatpickr("#myID", {});

// Create multiple instances
flatpickr(".anotherSelector");
{{< /code-highlight >}}

</div>

  </li>
</ul>

<!-------------------- Basic examples -------------------->

## Basic examples

<!-- Date picker -->

### Date picker

Basic date picker example.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-date" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Basic
    flatpickr('#flatpickr-date', {
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-- Time picker -->

### Time picker

Basic time picker example.

```html
<input type="text" class="input max-w-sm" placeholder="HH:MM" id="flatpickr-time" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Time
    flatpickr('#flatpickr-time', {
      enableTime: true,
      noCalendar: true,
      dateFormat: 'H:i'
    })
  })
</script>
```

<!-------------------- Types -------------------->

## Types

<!-- Default -->

### Default

Default datepicker.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-default" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Default Type
    flatpickr('#flatpickr-default', {
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-- Floating -->

### Floating

Floating label example.

```html
<div class="input-floating max-w-sm">
  <input type="text" placeholder="YYYY-MM-DD" class="input" id="flatpickr-floating" />
  <label class="input-floating-label" for="flatpickr-floating">Date</label>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // floating Type
    flatpickr('#flatpickr-floating', {
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="flatpickrStateSuccess">Date</label>
  <input type="text" placeholder="YYYY-MM-DD" class="input is-valid flatpickr-success" id="flatpickrStateSuccess" />
  <span class="helper-text">Helper text</span>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="YYYY-MM-DD" class="input is-valid flatpickr-success" id="flatpickrFloatingStateSuccess" />
  <label class="input-floating-label" for="flatpickrFloatingStateSuccess">Date</label>
  <span class="helper-text ps-3">Helper text</span>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Success Date Picker
    flatpickr('.flatpickr-success', {
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="flatpickrStateError">Date</label>
  <input type="text" placeholder="John Doe" class="input is-invalid flatpickr-error" id="flatpickrStateError" />
  <span class="helper-text">Helper text</span>
</div>

<div class="input-floating max-w-sm">
  <input type="text" placeholder="John Doe" class="input is-invalid flatpickr-error" id="flatpickrFloatingStateError" />
  <label class="input-floating-label" for="flatpickrFloatingStateError">Date</label>
  <span class="helper-text ps-3">Helper text</span>
</div>

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Error  Date Picker
    flatpickr('.flatpickr-error', {
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- DateTime picker -->

### DateTime picker

Example showcasing a picker with both date and time selection.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD HH:MM" id="flatpickr-date-time" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Date Time
    flatpickr('#flatpickr-date-time', {
      enableTime: true,
      dateFormat: 'Y-m-d H:i'
    })
  })
</script>
```

<!-- Multiple dates picker -->

### Multiple dates picker

Example demonstrating how to select multiple dates.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD, YYYY-MM-DD" id="flatpickr-multiple-date" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Multiple Date
    flatpickr('#flatpickr-multiple-date', {
      mode: 'multiple',
      dateFormat: 'Y-m-d'
    })
  })
</script>
```

<!-- Range picker -->

### Range picker

Select range of date.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD to YYYY-MM-DD" id="flatpickr-range" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Range Date Picker
    flatpickr('#flatpickr-range', {
      mode: 'range'
    })
  })
</script>
```

<!-- Human friendly -->

### Human friendly

Human Friendly date picker example.

```html
<input type="text" class="input max-w-sm" placeholder="Month DD, YYYY" id="flatpickr-human-friendly" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Human Friendly
    flatpickr('#flatpickr-human-friendly', {
      altInput: true,
      altFormat: 'F j, Y',
      dateFormat: 'Y-m-d'
    })
  })
</script>
```

<!-- Inline picker -->

### Inline picker

Basic inline picker example.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-inline" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Inline Date Picker
    flatpickr('#flatpickr-inline', {
      inline: true,
      allowInput: false,
      monthSelectorType: 'static'
    })
  })
</script>
```

<!-- Disabled dates -->

### Disabled dates

The example below demonstrates how to disable a specific date range.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-disabled-range" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Disable Date Picker
    const fromDate = new Date(Date.now() - 3600 * 1000 * 48)
    const toDate = new Date(Date.now() + 3600 * 1000 * 48)
    flatpickr('#flatpickr-disabled-range', {
      dateFormat: 'Y-m-d',
      disable: [
        {
          from: fromDate.toISOString().split('T')[0],
          to: toDate.toISOString().split('T')[0]
        }
      ]
    })
  })
</script>
```

<!-- Localization -->

### Localization

The date picker below has been localized to display months and days in Russian. For more information, please refer to the official documentation on <a href="https://flatpickr.js.org/localization/" target="_blank" class="link link-primary">localization</a>.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-localization" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Localization
    flatpickr('#flatpickr-localization', {
      locale: 'ru'
    })
  })
</script>
```

<!-- Display week numbers -->

### Display week numbers
Example displaying week number.

```html
<input type="text" class="input max-w-sm" placeholder="YYYY-MM-DD" id="flatpickr-week-number" />

<!-- Js -->
<script>
  window.addEventListener('load', function () {
    // Week Numbers
    flatpickr('#flatpickr-week-number', {
      weekNumbers: true,
      monthSelectorType: 'static'
    })
  })
</script>
```
