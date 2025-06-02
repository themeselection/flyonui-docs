# File input

File inputs enable users to choose files from their device, allowing them to upload documents, images, or other types of files.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| input | component | Base class for form input. |
| input-floating | component | Base class for floating form input. |
| label-text | part | Base class for title label text. |
| input-floating-label | part | Floats the label to the top. |
| helper-text | part | Base class for helper label text. |
| is-valid | state | Adds success style to the input. |
| is-invalid | state | Adds error style to the input. |
| file:{tw-utility-class} | modifier | Adds tailwind classes to update file input. |
| input-xs | size | Input with Extra small size. |
| input-sm | size | Input with Smaller size. |
| input-md | size | Input with medium(default) size. |
| input-lg | size | Input with Larger size. |
| input-xl | size | Input with Extra large size. |


<!-------------------- Basic example -------------------->

## Basic example

<!--  Default  -->

### Default

Basic file input example.

```html
<input type="file" class="input max-w-sm" aria-label="file-input" />
```

<!--  Label  -->

### Label

Basic file input example with label.

```html
<div class="max-w-sm">
  <label class="label-text" for="fileInputLabel"> Pick a file </label>
  <input type="file" class="input" id="fileInputLabel" />
</div>
```

<!-------------------- Size -------------------->

## Size

<!--  File input sizes  -->

### File input sizes

Add responsive class `input-{size}` where `{size} = xs|sm|md|lg|xl` for file input of different sizes.

```html
<input type="file" class="input max-w-sm input-xs" aria-label="file-input" />
<input type="file" class="input max-w-sm input-sm" aria-label="file-input" />
<input type="file" class="input max-w-sm" aria-label="file-input" />
<input type="file" class="input max-w-sm input-lg" aria-label="file-input" />
<input type="file" class="input max-w-sm input-xl" aria-label="file-input" />
```

<!-------------------- Types -------------------->

## Types

<!-- Default -->

### Default

Default type.

```html
<div class="max-w-sm">
  <label class="label-text" for="inpuFileTypeDefault"> Pick a file </label>
  <input type="file" class="input" id="inpuFileTypeDefault" />
</div>
```

<!-- Floating label -->

### Floating label

Floating label example.

```html
<div class="max-w-sm input-floating">
  <input type="file" placeholder="John Doe" class="input" id="inpuFileTypeFloating" />
  <label class="input-floating-label" for="inpuFileTypeFloating">Upload</label>
</div>
```

<!-------------------- Validation states -------------------->

## Validation states

<!-- Success state -->

### Success state

Success state can be show using `is-valid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="fileInputStateSuccess"> Pick a file </label>
  <input type="file" class="input is-valid" id="fileInputStateSuccess" />
  <span class="helper-text">Helper text</span>
</div>
<div class="input-floating max-w-sm">
  <input type="file" placeholder="John Doe" class="input is-valid" id="fileInputStateSuccessFloating" />
  <label class="input-floating-label" for="fileInputStateSuccessFloating">Upload</label>
 <span class="helper-text">Helper text</span>
</div>
```

<!-- Error state -->

### Error state

Error state can be show using `is-invalid` class.

```html
<div class="max-w-sm">
  <label class="label-text" for="fileInputStateError"> Pick a file </label>
  <input type="file" class="input is-invalid" id="fileInputStateError" />
  <span class="helper-text">Helper text</span>
</div>
<div class="input-floating max-w-sm">
  <input type="file" placeholder="John Doe" class="input is-invalid" id="fileInputStateErrorFloating" />
  <label class="input-floating-label" for="fileInputStateErrorFloating">Upload</label>
  <span class="helper-text">Helper text</span>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!--  File input with button  -->

### File input with button

The `file:` prefix in Tailwind allows us to style the `::file-selector-button`, and it can be combined with the `btn` class.

```html
<input type="file" class="block cursor-pointer text-sm file:uppercase file:text-bg-primary file:px-4 file:h-9.5 file:rounded-field cursor-pointer file:font-medium file:text-base file:me-3" aria-label="file-input" />
```

<!--  Disabled  -->

### Disabled

Add the `disabled` boolean attribute on an file input to remove pointer events, and prevent focusing.

```html
<input type="file" class="input max-w-sm" aria-label="file-input" disabled />
```

<!--  Helper text and label  -->

### Helper text and label

Placement of helper text and label.

```html
<div class="max-w-sm">
  <label class="label-text" for="fileInputHelperText"> Pick a file </label>
  <input type="file" class="input" id="fileInputHelperText" />
  <span class="helper-text">Helper text</span>
</div>
```

<!--  Multiple files  -->

### Multiple files

Add `multiple` attribute to select more then 1 file.

```html
<input type="file" class="input max-w-sm" aria-label="file-input" multiple />
```

<!-- Avatar -->

### Avatar

The following example showcases a file input with an avatar.

```html
<div class="flex items-center gap-2 max-sm:flex-wrap">
  <div class="avatar">
    <div class="size-14 rounded-full">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="Avatar" />
    </div>
  </div>
  <input type="file" class="file:text-bg-primary file:px-4 file:h-9.5 cursor-pointer file:font-medium file:text-base block text-sm file:me-3 file:rounded-full file:uppercase" aria-label="file-input" />
</div>
```
