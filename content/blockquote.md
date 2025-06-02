# Blockquote

The blockquote component serves as a tool to incorporate quoted text from an external source, ideal for testimonials, reviews, and quotes within an article.

<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Basic blockquote example.

```html
<blockquote class="relative p-4">
  <span class="icon-[tabler--quote] text-base-300/20 absolute -start-3 -top-3 size-16 rotate-180 rtl:rotate-0"></span>

  <div class="relative z-1">
    <p class="text-base-content text-lg">
      <em>
        The blockquote element is ideal for showcasing well-known quotes within content. It's commonly used for
        testimonials, reviews, and notable quotes in articles.
      </em>
    </p>
  </div>
</blockquote>
```

<!-------------------- Alignment -------------------->

## Alignment

<!-- Center align -->

### Center align

An example of a centered blockquote.

```html
<blockquote class="relative mx-auto p-4 text-center">
  <span class="icon-[tabler--quote] text-base-300/20 absolute -top-3 start-2 size-16 rotate-180 rtl:rotate-0"></span>

  <div class="relative z-1">
    <p class="text-base-content text-lg">
      <em>
        The blockquote element is ideal for showcasing well-known quotes within content. It's commonly used for
        testimonials, reviews, and notable quotes in articles.
      </em>
    </p>
  </div>
</blockquote>
```

<!-- Right align -->

### Right align

An example of a end blockquote.

```html
<blockquote class="relative ms-auto p-4 text-end">
  <span class="icon-[tabler--quote] text-base-300/20 absolute -top-3 start-6 size-16 rotate-180 rtl:rotate-0"></span>

  <div class="relative z-1">
    <p class="text-base-content text-lg">
      <em>
        The blockquote element is ideal for showcasing well-known quotes within content. It's commonly used for
        testimonials, reviews, and notable quotes in articles.
      </em>
    </p>
  </div>
</blockquote>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Naming a source -->

### Naming a source

Labeling a source with a name.

```html
<blockquote class="relative p-4">
  <span class="icon-[tabler--quote] text-base-300/20 absolute -start-3 -top-3 size-16 rotate-180 rtl:rotate-0"></span>

  <div class="relative z-1">
    <p class="text-base-content text-lg">
      <em>
        The blockquote element is ideal for showcasing well-known quotes within content. It's commonly used for
        testimonials, reviews, and notable quotes in articles.
      </em>
    </p>
  </div>
  <footer class="mt-4">
    <div class="text-base-content/50 text-base font-semibold">~ Shamus Tuttle</div>
  </footer>
</blockquote>
```

<!-- With avatar -->

### With avatar

Labeling a source with an avatar.

```html
<blockquote class="relative p-4">
  <span class="icon-[tabler--quote] text-base-300/20 absolute -start-3 -top-3 size-16 rotate-180 rtl:rotate-0"></span>

  <div class="relative z-1">
    <p class="text-base-content text-lg">
      <em>
        The blockquote element is ideal for showcasing well-known quotes within content. It's commonly used for
        testimonials, reviews, and notable quotes in articles.
      </em>
    </p>
  </div>
  <footer class="mt-4 flex items-center">
    <div class="avatar">
      <div class="size-10 rounded-full">
        <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="avatar" />
      </div>
    </div>
    <div class="ms-4">
      <div class="text-base-content text-base font-semibold">Shamus Tuttle</div>
      <div class="text-base-content/50 text-xs">Source title</div>
    </div>
  </footer>
</blockquote>
```
