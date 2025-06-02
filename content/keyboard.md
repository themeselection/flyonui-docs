# keyboard

The Keyboard component showcases keyboard keys, allowing you to present custom-designed keys that enhance the overall user interface.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| kbd | component | Base class for the keyboard component. |
| kbd-xs | size | Keyboard with extra small size. |
| kbd-sm | size | Keyboard with small size. |
| kbd-md | size | Keyboard with medium(default) size. |
| kbd-lg | size | Keyboard with large size. |
| kbd-xl | size | Keyboard with extra large size. |


<!-------------------- Variant -------------------->

## Basic variant

<!-- Default kbd -->

### Default kbd

Use the component class `kbd` to display the keyboard shortcut.

```html
<kbd class="kbd">A</kbd>
<kbd class="kbd">B</kbd>
<kbd class="kbd">C</kbd>
<kbd class="kbd">D</kbd>
```

<!-------------------- Sizes -------------------->

## Sizes

<!-- Size variants -->

### Size variants

Add responsive class `kbd-{size}` where `{size} = xs|sm|md|lg|xl` for different sizes.

```html
<kbd class="kbd kbd-xs">Ctrl</kbd>
<kbd class="kbd kbd-sm">Ctrl</kbd>
<kbd class="kbd">Ctrl</kbd>
<kbd class="kbd kbd-lg">Ctrl</kbd>
<kbd class="kbd kbd-xl">Ctrl</kbd>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- In text -->

### In text

Use kbd's in text to illustrate keyboard shortcuts.

```html
<p>Press <kbd class="kbd kbd-sm">Enter</kbd> to continue.</p>
```

<!-- Key combinations -->

### Key combinations

Use the `+` sign to display key combinations.

```html
<kbd class="kbd">Ctrl</kbd>+<kbd class="kbd">Shift</kbd>+<kbd class="kbd">Delete</kbd>
```

<!-- Function keys -->

### Function keys

Use special characters to display function keys.

```html
<kbd class="kbd">⌘</kbd>
<kbd class="kbd">⌥</kbd>
<kbd class="kbd">⇧</kbd>
<kbd class="kbd">⌃</kbd>
<kbd class="kbd">F1</kbd>
<kbd class="kbd">F2</kbd>
<kbd class="kbd">F3</kbd>
<kbd class="kbd">F4</kbd>
```

<!-- A full keyboard -->

### A full keyboard

Use the `flex` and `justify-center` utility classes to display a full keyboard.

```html
<div class="flex justify-center gap-1 w-full max-sm:*:kbd-sm">
  <kbd class="kbd">q</kbd>
  <kbd class="kbd">w</kbd>
  <kbd class="kbd">e</kbd>
  <kbd class="kbd">r</kbd>
  <kbd class="kbd">t</kbd>
  <kbd class="kbd">y</kbd>
  <kbd class="kbd">u</kbd>
  <kbd class="kbd">i</kbd>
  <kbd class="kbd">o</kbd>
  <kbd class="kbd">p</kbd>
</div>

<div class="flex justify-center gap-1 w-full max-sm:*:kbd-sm">
  <kbd class="kbd">a</kbd>
  <kbd class="kbd">s</kbd>
  <kbd class="kbd">d</kbd>
  <kbd class="kbd">f</kbd>
  <kbd class="kbd">g</kbd>
  <kbd class="kbd">h</kbd>
  <kbd class="kbd">j</kbd>
  <kbd class="kbd">k</kbd>
  <kbd class="kbd">l</kbd>
</div>

<div class="flex justify-center gap-1 w-full max-sm:*:kbd-sm">
  <kbd class="kbd">z</kbd>
  <kbd class="kbd">x</kbd>
  <kbd class="kbd">c</kbd>
  <kbd class="kbd">v</kbd>
  <kbd class="kbd">b</kbd>
  <kbd class="kbd">n</kbd>
  <kbd class="kbd">m</kbd>
  <kbd class="kbd">,</kbd>
</div>
```

<!-- Arrow keys -->

### Arrow keys

Use the `flex` and `justify-center` utility classes to display arrow keys.

```html
<div class="flex w-full justify-center">
  <kbd class="kbd"><span class="icon-[tabler--caret-up-filled] size-5"></span></kbd>
</div>
<div class="flex w-full justify-center gap-12">
  <kbd class="kbd"><span class="icon-[tabler--caret-left-filled] size-5"></span></kbd>
  <kbd class="kbd"><span class="icon-[tabler--caret-right-filled] size-5"></span></kbd>
</div>
<div class="flex w-full justify-center">
  <kbd class="kbd"><span class="icon-[tabler--caret-down-filled] size-5"></span></kbd>
</div>
```

<!-- Number keys -->

### Number keys

Use kbd with numbers to display number keys.

```html
<kbd class="kbd">0</kbd>
<kbd class="kbd">1</kbd>
<kbd class="kbd">2</kbd>
<kbd class="kbd">3</kbd>
<kbd class="kbd">4</kbd>
<kbd class="kbd">5</kbd>
<kbd class="kbd">6</kbd>
<kbd class="kbd">7</kbd>
<kbd class="kbd">8</kbd>
<kbd class="kbd">9</kbd>
```
