# Select

A select element is utilized to choose a value from a range of options.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| select | component | Basic select field. |
| select-floating | component | Floating select field. |
| select-floating-label | part | Floats the label to the top. |
| label-text | part | For label. |
| helper-text | part | For helper text. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| select-xs | size | Extra small select size. |
| select-sm | size | Smaller select size. |
| select-md | size | Medium(default) select size. |
| select-lg | size | Larger select size. |
| select-xl | size | Extra large select size. |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic select example.

```html
<select class="select max-w-sm appearance-none" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>
```

<!-------------------- Type -------------------->

## Type

<!-- Default -->

### Default

The `<select>` element's customization options are primarily confined to its initial appearance. Due to browser constraints, modifications to the appearance of `<option>` elements within the dropdown are not possible.

```html
<div class="w-96">
  <label class="label-text" for="favorite-simpson">Pick your favorite Movie</label>
  <select class="select" id="favorite-simpson">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
</div>
```

<!-- Floating label -->

### Floating label

The `label` remains in its floated position at all times, unlike with `input` elements. Pair `select-floating` with your `select` element and `select-floating-label` for the label.

```html
<div class="select-floating w-96">
  <select class="select" aria-label="Select floating label" id="selectFloating">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloating">Pick your favorite Movie</label>
</div>
```

<!-------------------- Size -------------------->

## Size

<!-- Default -->

### Default

Add responsive class `select-{size}` where `{size} = xs|sm|md|lg|xl` for select of different sizes.

```html
<select class="select select-xs max-w-sm" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<select class="select select-sm max-w-sm" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<select class="select max-w-sm" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<select class="select select-lg max-w-sm" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<select class="select select-xl max-w-sm" aria-label="select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>
```

<!-- Floating label -->

### Floating label

Add responsive class `select-{size}` where `{size} = xs|sm|md|lg|xl` for select of different sizes.

```html
<div class="select-floating max-w-sm">
  <select class="select select-xs" id="selectFloatingExtraSmall" aria-label="floating label">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingExtraSmall">Pick your favorite Movie</label>
</div>

<div class="select-floating max-w-sm">
  <select class="select select-sm" id="selectFloatingSmall" aria-label="floating label">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingSmall">Pick your favorite Movie</label>
</div>

<div class="select-floating max-w-sm">
  <select class="select" id="selectFloatingDefault" aria-label="floating label">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingDefault">Pick your favorite Movie</label>
</div>

<div class="select-floating max-w-sm">
  <select class="select select-lg" id="selectFloatingLarge" aria-label="floating label">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingLarge">Pick your favorite Movie</label>
</div>

<div class="select-floating max-w-sm">
  <select class="select select-xl" id="selectFloatingExtraLarge" aria-label="floating label">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingExtraLarge">Pick your favorite Movie</label>
</div>
```

<!-------------------- Select group -------------------->
## Select group

<!-- Leading icons -->

### Leading icons

Add a leading icon inside select. There are no tailing icons for select

```html
<div class="w-96 select">
 <span class="icon-[tabler--movie] text-base-content/80 my-auto size-5 shrink-0"></span>
  <label class="sr-only" for="favorite-simpson">Pick your favorite Movie</label>
  <select id="favorite-simpson">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
</div>

<div class="select max-w-sm">
  <span class="icon-[tabler--movie] text-base-content/80 my-auto size-5 shrink-0"></span>
  <div class="select-floating">
    <select aria-label="Select floating label" id="selectFloating">
      <option>The Godfather</option>
      <option>The Shawshank Redemption</option>
      <option>Pulp Fiction</option>
      <option>The Dark Knight</option>
      <option>Schindler's List</option>
    </select>
    <label class="select-floating-label" for="selectFloating">Pick your favorite Movie</label>
  </div>
</div>
```


<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state which can be added by using class `is-valid`.

```html
<div class="max-w-sm">
  <label class="label-text" for="selectStateSuccessDefault"> Full Name </label>
  <select class="select is-valid" id="selectStateSuccessDefault">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <span class="helper-text">Helper text</span>
</div>

<div class="select-floating max-w-sm">
  <select class="select is-valid " id="selectStateSuccessFloating">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectStateSuccessFloating">Pick your favorite Movie</label>
  <span class="helper-text">Helper text</span>
</div>
```

<!-- Error state -->

### Error state

Error state can be added using class `is-invalid`.

```html
<div class="max-w-sm">
  <label class="label-text" for="selectStateErrorDefault"> Full Name </label>
  <select class="select is-invalid" id="selectStateErrorDefault">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <span class="helper-text">Helper text</span>
</div>

<div class="select-floating max-w-sm">
  <select class="select is-invalid" id="selectStateErrorFloating">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectStateErrorFloating">Pick your favorite Movie</label>
  <span class="helper-text ps-3">Helper text</span>
</div>
```

<!-------------------- Shape -------------------->

## Shape

<!-- Pilled select -->

### Pilled select

Use the `rounded-full` utility class to make select's circular. The default shape of the select but can be altered by using TailwindCSS <a href="https://tailwindcss.com/docs/border-radius" target="_blank" class="link link-primary">Border Radius</a>.

```html
<select class="select max-w-sm rounded-full" aria-label="Pilled select">
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<div class="select-floating max-w-sm">
  <select class="select rounded-full" id="selectFloatingPilled" aria-label="Pilled select">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectFloatingPilled">Pick your favorite Movie</label>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Label and helper text. -->

### Label and helper text

Use the `label-text` for the main label and `helper-text` class for helper text.
```html
<div class="w-96">
  <label class="label-text" for="selectHelperText"> Pick your favorite Movie </label>
  <select class="select" id="selectHelperText">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <span class="helper-text">Helper text</span>
</div>
```

<!-- Hidden label -->

### Hidden label

`label` elements hidden using the `.sr-only` class.

```html
<div class="w-96">
  <div class="label-text sr-only" for="selectHiddenLabel"> Pick your favorite Movie </div>
  <select class="select" id="selectHiddenLabel">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
</div>
```

<!-- Disabled -->

### Disabled

Disable a `select` element by adding the `disabled` attribute, making it non-selectable.

```html
<select class="select max-w-sm" aria-label="Disabled select" disabled>
  <option disabled selected>Pick your favorite Movie</option>
  <option>The Godfather</option>
  <option>The Shawshank Redemption</option>
  <option>Pulp Fiction</option>
  <option>The Dark Knight</option>
  <option>Schindler's List</option>
</select>

<div class="select-floating max-w-sm">
  <select class="select" id="selectDisabledFloating" aria-label="Disabled select" disabled>
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
  <label class="select-floating-label" for="selectDisabledFloating">Pick your favorite Movie</label>
</div>
```

<!-- Datalist -->

### Datalist

Associate a `datalist` element with an `input` to provide a list of suggested options, allowing users to select from predefined choices or enter a custom value.

```html
<div class="flex flex-col max-w-sm">
  <label for="exampleDataList" class="label-text">Datalist example</label>
  <input class="input" list="datalistOptions" id="exampleDataList" placeholder="Type to search..." />
  <datalist id="datalistOptions">
    <option value="San Francisco"></option>
    <option value="New York"></option>
    <option value="Seattle"></option>
    <option value="Los Angeles"></option>
    <option value="Chicago"></option>
  </datalist>
</div>
```

<!-- Multiple -->

### Multiple

Enable the selection of multiple options in a `select` element by adding the `multiple` attribute.

```html
<div class="max-w-sm">
  <label class="label-text" for="fav-movies">Pick your favorite Movies:</label>
  <select multiple class="select h-auto" size="4" name="fav-movies" id="fav-movies">
    <option>The Godfather</option>
    <option>The Shawshank Redemption</option>
    <option>Pulp Fiction</option>
    <option>The Dark Knight</option>
    <option>Schindler's List</option>
  </select>
</div>
```

<!-- Optgroup -->

### Optgroup

Utilize the `optgroup` element to group `option` elements together within a `select` dropdown, creating organized sections.

```html
<div class="w-96">
  <label class="label-text" for="technologies">Choose a technology:</label>
  <select class="select" name="technologies" id="technologies">
    <optgroup label="Frontend Technologies">
      <option value="html">HTML</option>
      <option value="css">CSS</option>
      <option value="javascript">JavaScript</option>
    </optgroup>
    <optgroup label="Backend Technologies">
      <option value="nodejs">Node.js</option>
      <option value="python">Python</option>
      <option value="java">Java</option>
    </optgroup>
  </select>
</div>
```
