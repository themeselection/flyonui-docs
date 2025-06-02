# Phone

The phone mockup presents a design that resembles an iPhone, showcasing its interface and features in a realistic format.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| mockup-phone | component | Container element. |
| mockup-phone-camera | part | Add iphone dynamic island. |
| mockup-phone-display | part | Content container. |


<!-------------------- Basic examples -------------------->

## Basic examples

<!-- Default -->

### Default

Basic example of phone.

Use the `mockup-phone` component class to contain the phone mockup. The `mockup-phone-camera` class introduces dynamic island UI elements. Meanwhile, the `mockup-phone-display` class serves as a container for displaying items.

```html
<div class="mockup-phone">
  <div class="mockup-phone-camera"></div> 
  <div class="mockup-phone-display bg-base-200">
    <div class="h-142 w-80 grid place-content-center">Hi.</div>
  </div>
</div>
```

<!-- Image -->

### Image

This demonstrates how we use images as display.

```html
<div class="mockup-phone">
  <div class="mockup-phone-camera"></div> 
  <div class="mockup-phone-display flex justify-center">
    <div class="h-142 w-80"><img class="size-full object-cover" src="https://cdn.flyonui.com/fy-assets/components/iphone/image.png" alt="phone background" /></div>
  </div>
</div>
```
