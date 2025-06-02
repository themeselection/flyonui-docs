# Customize components

Quickly personalize and easily modify components within just a few minutes.

<!-------------------- How to customize FlyonUI? -------------------->

{{< headsingle addClass="!mt-px" level="2" >}} How to customize FlyonUI? {{< /headsingle >}}

FlyonUI components come with many built-in variants, making it unlikely that you'll need to customize anything. However, if needed, you can still modify components in various ways:

- For example, to customize this button:

```html
<button class="btn">Button</button>
```

<button class="btn mt-4">Button</button>

<!-- Use FlyonUI utility classes: -->

#### 1. Use FlyonUI utility classes:

```html
<button class="btn btn-primary">One</button>
<button class="btn btn-accent btn-gradient">Two</button>
<button class="btn btn-accent btn-outline">Three</button>
```

<div class="flex items-center gap-4 my-4">
  <button class="btn btn-primary">One</button>
  <button class="btn btn-accent btn-gradient">Two</button>
  <button class="btn btn-error btn-outline">Three</button>
</div>

<!-- Use Tailwind's utility classes: -->

#### 2. Use Tailwind's utility classes:

```html
<button class="btn rounded-full">One</button>
<button class="btn rounded-none px-16">Two</button>
```

<div class="flex items-center gap-4 my-4">
  <button class="btn rounded-full">One</button>
  <button class="btn rounded-none px-16">Two</button>
</div>

<!-- Customize via CSS using Tailwind's `@apply` directive: -->

#### 3. Customize via `@apply` directive:

```php
.btn {
  @apply rounded-full;
}
```

<br/>

<!-- Other options: -->

#### 4. Other options:

- [Create your own theme](customization/themes/).
- Disable FlyonUI's design decisions and use the [unstyled (skeleton)](customization/config/#styled) version of FlyonUI.
