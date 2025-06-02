# Browser

The browser mockup features a design that resembles a browser window, complete with typical interface elements and layout.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| mockup-browser | component | Container element. |
| mockup-browser-toolbar | part | The toolbar that can include address bar or other things. |


<!-------------------- Basic examples -------------------->

## Basic examples

<!-- Bordered -->

### Bordered

The `mockup-browser` class serves as a container for the browser mockup, while `mockup-browser-toolbar` acts as a container for the header links within the mockup.

```html
<div class="mockup-browser border border-neutral/30">
  <div class="mockup-browser-toolbar">
    <div class="input border border-neutral/30">https://flyonui.com</div>
  </div>
  <div class="flex justify-center px-4 py-16 border-t border-neutral/30">Hello!</div>
</div>
```

<!-- Background color -->

### Background color

Browser mockup featuring a customizable background color. Update it to your preference using the `bg-*` Tailwind utility class.

```html
<div class="mockup-browser bg-base-300/40">
  <div class="mockup-browser-toolbar">
    <div class="input bg-base-200">https://flyonui.com</div>
  </div>
  <div class="flex justify-center px-4 py-16 bg-base-200">Hello!</div>
</div>
```

<!-- Image -->

### Image

Browser mockup featuring a image.

```html
<div class="mockup-browser bg-base-300/40">
  <div class="mockup-browser-toolbar">
    <div class="input bg-base-200">https://flyonui.com</div>
  </div>
  <div class="flex h-80 justify-center"><img class="w-full object-cover" src="https://cdn.flyonui.com/fy-assets/components/carousel/image-14.png" alt="browser background" /></div>
</div>
```
