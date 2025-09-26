# Window

The window mockup presents content inside a styled container that mimics a standard OS window, ideal for showcasing apps, websites, or UI previews.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| mockup-window | component | Container element. |


<!-------------------- Basic examples -------------------->

## Basic examples

<!-- Bordered -->

### Bordered

Wtilize the `mockup-window` class as a container for the window mockup and apply Tailwind utility classes such as `border` and `background-color` for styling.

```html
<div class="mockup-window border border-base-content/20">
  <div class="flex justify-center px-4 py-16 border-t border-base-content/20">Hello!</div>
</div>
```

<!-- Background color -->

### Background color

Window mockup featuring a customizable background color. Update it to your preference using the `bg-*` Tailwind utility class.

```html
<div class="mockup-window border border-base-content/20 bg-base-300/40">
  <div class="flex justify-center px-4 py-16 bg-base-200">Hello!</div>
</div>
```

<!-- Image -->

### Image

Window mockup featuring a image.

```html
<div class="mockup-window border border-base-content/20 bg-base-200">
   <div class="flex justify-center h-80"><img class="w-full object-cover" src="https://cdn.flyonui.com/fy-assets/components/carousel/image-21.png" alt="window background" /></div>
</div>
```
