# Timeline

Build FlyonUI timelines with Tailwind CSS. Create responsive, chronological event displays for storytelling in web projects.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| timeline | component | Container element. |
| timeline-start | part | The content inside `<li>` that will be at the start direction. |
| timeline-middle | part | The content inside `<li>` that will be at the middle. |
| timeline-end | part | The content inside `<li>` that will be at the end direction. |
| timeline-snap-icon | modifier | Snaps the icon to the start instead of middle. |
| timeline-box | modifier | Applies a box style to timeline-start or timeline-end. |
| timeline-compact | modifier | Forces all items on one side. |
| timeline-centered | modifier | Sets content position in grid for centered timeline at start. |
| timeline-shift | modifier | Facilitates content adjustment on smaller screens. |
| timeline-vertical | direction | Shows the timeline vertically. |
| timeline-horizontal | direction | Shows the timeline horizontally. |


<!-------------------- Alignment -------------------->

## Alignment

<!--  Horizontal  -->

### Horizontal

Apply the `timeline` class to the `<ul>` element to establish the foundation for the timeline component. Within the timeline, utilize `<li>` elements to represent individual timeline items.

Use the component classes `timeline-start`, `timeline-middle`, or `timeline-end` to position elements within the timeline grid at the top, center, or end respectively.

Use `<hr />` as first and last child of `<li>` for path of timeline.

Apply the modifier class `timeline-box` to give any specific timeline item a boxed style.

Utilize the provided example for crafting a horizontal timeline component.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!--  Vertical  -->

### Vertical

Incorporate the responsive class `timeline-vertical` to create a vertical timeline component.

Use the component classes `timeline-start`, `timeline-middle`, or `timeline-end` to position elements within the timeline grid at the start, center, or end respectively.

```html
<ul class="timeline timeline-vertical">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-------------------- Types -------------------->

## Types

<!-- Basic -->

### Basic

The example provided showcases a basic type of timeline.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-- Icons -->

### Icons

The below example showcases a type of timeline with icons.

```html
<ul class="timeline timeline-vertical overflow-x-auto lg:timeline-horizontal">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr class="bg-primary" />
  </li>
  <li>
    <hr class="bg-primary" />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr class="bg-primary" />
  </li>
  <li>
    <hr class="bg-primary" />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr class="bg-primary" />
  </li>
  <li>
    <hr class="bg-primary" />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr class="bg-primary" />
  </li>
  <li>
    <hr class="bg-primary" />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="badge badge-secondary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--target] text-secondary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-------------------- Content position -------------------->

## Content position

<!--  Horizontal timeline  -->

### Horizontal timeline

Utilize the following examples to determine the positioning of content within the horizontal timeline component.

<!-- Content on both sides -->

#### Content on both sides

Use the provided example of a timeline featuring content on both sides.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-- Content only on bottom -->

#### Content only on bottom

Use the provided example of a timeline featuring content only on bottom.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-- Content only on top -->

#### Content only on top

Use the provided example of a timeline featuring content only on top.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-start timeline-box">Macintosh PC</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iMac</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPod</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPhone</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Apple Watch</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Vision Pro</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
  </li>
</ul>
```

<!-- Content on alternate sides -->

#### Content on alternate sides

Use the provided example of a timeline featuring content on alternate sides.

```html
<ul class="timeline overflow-x-auto">
  <li>
    <div class="timeline-start timeline-box">Macintosh PC</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPod</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Apple Watch</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!--  Vertical timeline  -->

### Vertical timeline

Utilize the following examples to determine the positioning of content within the vertical timeline component.

<!-- Content on both sides -->

#### Content on both sides

Use the provided example of a timeline featuring content on both sides.

```html
<ul class="timeline timeline-vertical">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-- Content only on start -->

#### Content only on start

Use the provided example of a timeline featuring content only on start.

```html
<ul class="timeline timeline-vertical">
  <li>
    <div class="timeline-start timeline-box">Macintosh PC</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iMac</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPod</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPhone</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Apple Watch</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Vision Pro</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
  </li>
</ul>
```

<!-- Content only on end -->

#### Content only on end

Use the provided example of a timeline featuring content only on end.

```html
<ul class="timeline timeline-vertical timeline-compact">
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-- Content on alternate sides -->

#### Content on alternate sides

Use the provided example of a timeline featuring content on alternate sides.

```html
<ul class="timeline timeline-vertical">
  <li>
    <div class="timeline-start timeline-box">Macintosh PC</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">iPod</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start timeline-box">Apple Watch</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Responsive -->

### Responsive

Use TailwindCSS classes for <a href="https://tailwindcss.com/docs/responsive-design#targeting-a-breakpoint-range" target="_blank" class="link link-primary">responsive design</a>, such as `sm:`, `md:`, `lg:`, `xl:`, and `2xl:`, along with the responsive class `timeline-horizontal`, to switch the timeline alignment to horizontal at specific breakpoints or vice the versa.

```html
<ul class="timeline timeline-vertical lg:timeline-horizontal">
  <li>
    <div class="timeline-start text-base-content font-medium">1984</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Macintosh PC</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">1998</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iMac</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2001</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPod</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2007</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">iPhone</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2015</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Apple Watch</div>
    <hr />
  </li>
  <li>
    <hr />
    <div class="timeline-start text-base-content font-medium">2024</div>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end timeline-box">Vision Pro</div>
  </li>
</ul>
```

<!--  Hoverable  -->

### Hoverable

Utilize the provided example for a timeline item to implement a background change on hover.

```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <!-- Hoverable timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end hover:bg-base-200/50 mb-0 ms-1 w-3/4 rounded-lg p-4 pt-1">
      <div class="text-base-content mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        12 Invoices have been paid
        <span class="text-base-content/50 text-sm font-normal">12 mins ago</span>
      </div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-text btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr />
  </li>
  <!-- /Hoverable timeline item 1-->
  <!-- Hoverable timeline item 2-->
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-success/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-success size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end hover:bg-base-200/50 mb-0 ms-1 w-3/4 rounded-lg p-4 pt-1">
      <div class="text-base-content mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Client meeting
        <span class="text-base-content/50 text-sm font-normal">45 mins ago</span>
      </div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /Hoverable timeline item 2-->
  <!-- Hoverable timeline item 3-->
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-info/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-info size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end hover:bg-base-200/50 mb-0 ms-1 w-3/4 rounded-lg p-4 pt-1">
      <div class="text-base-content mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Create a new project for client
        <span class="text-base-content/50 text-sm font-normal">2 days ago</span>
      </div>
      <p class="mb-2">6 team members in a project</p>
      <div class="avatar-group pull-up -space-x-4">
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-8">
            <span>+3</span>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /Hoverable timeline item 3-->
</ul>
```

<!-- Informative timeline -->

### Informative timeline

The Informative timeline provides detailed information about each timeline item, including timestamps and descriptions.

<!--  Styled  -->

#### Styled

The below example showcases a basic informative timeline.

```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        12 Invoices have been paid
        <span class="text-base-content/50 text-sm font-normal">12 mins ago</span>
      </div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-soft btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr />
  </li>
  <!-- /timeline item 1-->

  <!-- timeline item 2-->
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-success/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-success size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Client meeting
        <span class="text-base-content/50 text-sm font-normal">45 mins ago</span>
      </div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 2-->

  <!-- timeline item 3-->
  <li>
    <hr />
    <div class="timeline-middle">
      <span class="bg-info/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-info size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Create a new project for client
        <span class="text-base-content/50 text-sm font-normal">2 days ago</span>
      </div>
      <p class="mb-2">6 team members in a project</p>
      <div class="avatar-group pull-up -space-x-4">
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-8">
            <span>+3</span>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 3-->
</ul>
```

<!--  With Icons  -->

#### With Icons

The below example showcases a informative timeline with icons.

```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        12 Invoices have been paid
        <span class="text-base-content/50 text-sm font-normal">12 mins ago</span>
      </div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-soft btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr class="bg-primary" />
  </li>
  <!-- /timeline item 1-->

  <!-- timeline item 2-->
  <li>
    <hr class="bg-primary" />
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Client meeting
        <span class="text-base-content/50 text-sm font-normal">45 mins ago</span>
      </div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr class="bg-primary" />
  </li>
  <!-- /timeline item 2-->

  <!-- timeline item 3-->
  <li>
    <hr class="bg-primary" />
    <div class="timeline-middle">
      <span class="bg-secondary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-secondary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 flex gap-2 font-medium max-sm:flex-col-reverse sm:items-center sm:justify-between" >
        Create a new project for client
        <span class="text-base-content/50 text-sm font-normal">2 days ago</span>
      </div>
      <p class="mb-2">6 team members in a project</p>
      <div class="avatar-group pull-up -space-x-4">
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-8">
            <span>+3</span>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 3-->
</ul>
```

<!--  Text in line  -->

### Text in line

Utilize the provided example for a timeline item where the text is positioned within the timeline path.

<!-- Styled -->

#### Styled

The examples below showcase a styled timeline with text positioned inline within the timeline path.

```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <span class="text-sm">April 1, 2024</span>
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">12 Invoices have been paid</div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-soft btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr />
  </li>
  <!-- /timeline item 1-->
  <span class="mt-2 text-sm">March 31, 2024</span>
  <!-- timeline item 2-->
  <li>
    <div class="timeline-middle">
      <span class="bg-success/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-success size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">Client meeting</div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 2-->
  <span class="mt-2 text-sm">March 31, 2024</span>
  <!-- timeline item 3-->
  <li>
    <div class="timeline-middle">
      <span class="bg-info/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-info size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">Create a new project for client</div>
      <p class="mb-2">6 team members in a project</p>
      <div class="avatar-group pull-up -space-x-4">
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-8">
            <span>+3</span>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 3-->
</ul>
```

<!-- With icon -->

#### With Icons

The examples below showcase a timeline with icons that positioned inline within the timeline path.

```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <span class="text-sm">April 1, 2024</span>
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">12 Invoices have been paid</div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-soft btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr class="bg-primary" />
  </li>
  <!-- /timeline item 1-->
  <span class="mt-2 text-sm">March 31, 2024</span>
  <!-- timeline item 2-->
  <li>
    <div class="timeline-middle">
      <span class="badge badge-primary size-4.5 rounded-full p-0">
        <span class="icon-[tabler--check] text-primary-content size-3.5"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">Client meeting</div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr class="bg-primary" />
  </li>
  <!-- /timeline item 2-->
  <span class="mt-2 text-sm">March 31, 2024</span>
  <!-- timeline item 3-->
  <li>
    <div class="timeline-middle">
      <span class="bg-secondary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-secondary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">Create a new project for client</div>
      <p class="mb-2">6 team members in a project</p>
      <div class="avatar-group pull-up -space-x-4">
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-8">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-8">
            <span>+3</span>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 3-->
</ul>
```

<!--  Centered timeline with icons  -->

### Centered timeline with icons

Apply the modifier class `timeline-centered` to adjust the content positions of `timeline-start` and `timeline-end`. Additionally, include the `timeline-shift` modifier class within the `<li>` element to facilitate content adjustment on smaller screens.

Apply the modifier class `timeline-snap-icon` to align icons to the start instead of the middle, and utilize the responsive class `timeline-compact` to consolidate all items on one side specifically for smaller screens.

Utilize the provided example for a centered timeline with icons.

```html
<ul class="timeline timeline-snap-icon max-md:timeline-compact timeline-vertical timeline-centered">
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle h-16">
      <span class="bg-error/20 flex size-8 items-center justify-center rounded-full">
        <span class="icon-[tabler--file] text-error size-5"></span>
      </span>
    </div>
    <div class="timeline-start me-4 mt-8 max-md:pt-2">
      <div class="text-base-content/50 text-sm font-normal">2 month’s ago</div>
    </div>
    <div class="timeline-end ms-4 mb-8">
      <div class="card">
        <div class="card-body gap-4">
          <h5 class="card-title text-lg">You've uploaded doc pdf to the FlyonUI</h5>
          <p>
            The process of recording the key project details and producing the documents that are required to implement
            it successfully. Simply put, it's an umbrella term which includes all the documents created over the course
            of the project.
          </p>
          <div class="card-actions">
            <button class="btn btn-sm btn-soft btn-secondary">
              <span class="icon-[tabler--file-type-pdf] text-error max-sm:hidden"></span>
              documentation.pdf
            </button>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 1-->
  <!-- timeline item 2-->
  <li class="timeline-shift">
    <div class="timeline-middle h-16">
      <span class="bg-success/20 flex size-8 items-center justify-center rounded-full">
        <span class="icon-[tabler--photo] text-success size-5"></span>
      </span>
    </div>
    <div class="timeline-end mt-6 px-1 md:mt-8">
      <div class="text-base-content/50 text-sm font-normal">24 day's ago</div>
    </div>
    <div class="timeline-start me-4 mb-8">
      <div class="card">
        <div class="card-body gap-4">
          <h5 class="card-title text-lg">Heather added 4 images to album</h5>
          <p>
            In the Select Image for Project dialog box, choose one of the following: Under the Upload New Image section
          </p>
          <div class="flex flex-wrap gap-4">
            <img src="https://cdn.flyonui.com/fy-assets/components/timeline/image-2.png" alt="timeline Image" class="w-16 rounded-sm" />
            <img src="https://cdn.flyonui.com/fy-assets/components/timeline/image-3.png" alt="timeline Image" class="w-16 rounded-sm" />
            <img src="https://cdn.flyonui.com/fy-assets/components/timeline/image-1.png" alt="timeline Image" class="w-16 rounded-sm" />
            <img src="https://cdn.flyonui.com/fy-assets/components/timeline/image-4.png" alt="timeline Image" class="w-16 rounded-sm" />
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 2-->
  <!-- timeline item 3-->
  <li>
    <div class="timeline-middle h-16">
      <span class="bg-warning/20 flex size-8 items-center justify-center rounded-full">
        <span class="icon-[tabler--star] text-warning size-5"></span>
      </span>
    </div>
    <div class="timeline-start me-4 mt-8 max-md:pt-2">
      <div class="text-base-content/50 text-sm font-normal">2 week's ago</div>
    </div>
    <div class="timeline-end ms-4 mb-8">
      <div class="card">
        <div class="card-body gap-4">
          <h5 class="card-title text-lg">Loretta wrote a review on FlyonUI</h5>
          <div class="flex items-center gap-2">
            <div class="avatar">
              <div class="size-9.5 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-6.png" alt="User Avatar" />
              </div>
            </div>
            <div>
              <p class="text-sm font-medium">Loretta Moore</p>
              <p class="text-sm">CTO of Airbnb</p>
            </div>
          </div>
          <div class="flex flex-wrap items-center justify-between gap-2 text-nowrap">
            <div class="text-warning flex items-center">
              <span class="icon-[tabler--star-filled] size-5"></span>
              <span class="icon-[tabler--star-filled] size-5"></span>
              <span class="icon-[tabler--star-filled] size-5"></span>
              <span class="icon-[tabler--star-filled] size-5"></span>
              <span class="icon-[tabler--star-filled] size-5"></span>
            </div>
            <span class="badge badge-soft badge-success uppercase">
              <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-6.png" alt="Anna" class="size-4.5 rounded-full" />
              Verified buyer
            </span>
          </div>
          <p>
            I wish I could select more than one main reason for rating this. I love how they constantly work on to make
            the template better. I am so thankful for this. Also, in the past, they had responded well to my tickets.
            Thank you for this great theme, for such an amazing support, for the better updates. I wish I could rate
            this for so many times. I highly recommend this template!
          </p>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 3-->
  <!-- timeline item 4-->
  <li class="timeline-shift">
    <div class="timeline-middle h-16">
      <span class="bg-info/20 flex size-8 items-center justify-center rounded-full">
        <span class="icon-[tabler--chart-pie] text-info size-5"></span>
      </span>
    </div>
    <div class="timeline-end mt-6 px-1 md:mt-8">
      <div class="text-base-content/50 text-sm font-normal">A week ago</div>
    </div>
    <div class="timeline-start me-4 mb-8 w-full">
      <div class="card">
        <div class="card-body gap-4">
          <h5 class="card-title text-lg">Julia stiles shared an earnings report</h5>
          <div>
            <div class="flex flex-wrap items-center gap-0.5 mb-1">
              <h4 class="text-base-content font-medium text-xl">$24,895</h4>
              <p class="text-success flex items-center">
                <span class="icon-[tabler--caret-up-filled] me-0.5"></span>
                10%
              </p>
            </div>
            <p class="text-sm">Compared to $84,325 last year</p>
          </div>
          <div class="space-y-4">
            <div class="flex flex-wrap items-center justify-between gap-2">
              <div class="flex items-center gap-3">
                <div class="avatar">
                  <div class="bg-base-content/5 size-10 rounded-md">
                    <img src="https://cdn.flyonui.com/fy-assets/components/card/icon-1.png" alt="Zipcar Logo" />
                  </div>
                </div>
                <div>
                  <div class="text-base-content font-medium">Zipcar</div>
                  <div class="text-sm">Vuejs, React & HTML</div>
                </div>
              </div>
              <div class="flex flex-col gap-2 max-sm:w-full">
                <p class="text-base-content">$24,895.65</p>
                <div class="progress" role="progressbar" aria-label="Progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
                  <div class="progress-bar progress-primary w-3/4"></div>
                </div>
              </div>
            </div>
            <div class="flex flex-wrap items-center justify-between gap-2">
              <div class="flex items-center gap-3">
                <div class="avatar">
                  <div class="bg-base-content/5 size-10 rounded-md">
                    <img src="https://cdn.flyonui.com/fy-assets/components/card/icon-2.png" alt="Bitbank logo" />
                  </div>
                </div>
                <div>
                  <div class="text-base-content font-medium">Bitbank</div>
                  <div class="text-sm">Sketch, Figma & XD</div>
                </div>
              </div>
              <div class="flex flex-col gap-2 max-sm:w-full">
                <p class="text-base-content">$8,6500.20</p>
                <div class="progress" role="progressbar" aria-label="Progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
                  <div class="progress-bar progress-info w-3/4"></div>
                </div>
              </div>
            </div>
            <div class="flex flex-wrap items-center justify-between gap-2">
              <div class="flex items-center gap-3">
                <div class="avatar">
                  <div class="bg-base-content/5 size-10 rounded-md">
                    <img src="https://cdn.flyonui.com/fy-assets/components/card/icon-3.png" alt="aviato logo" />
                  </div>
                </div>
                <div>
                  <div class="text-base-content font-medium">Aviato</div>
                  <div class="text-sm">HTML & Angular</div>
                </div>
              </div>
              <div class="flex flex-col gap-2 max-sm:w-full">
                <p class="text-base-content">$1,2450.80</p>
                <div class="progress" role="progressbar" aria-label="Progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
                  <div class="progress-bar progress-secondary w-3/4"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 4-->
  <!-- timeline item 5-->
  <li>
    <div class="timeline-middle h-16">
      <span class="bg-primary/20 flex size-8 items-center justify-center rounded-full">
        <span class="icon-[tabler--folder] text-primary size-5"></span>
      </span>
    </div>
    <div class="timeline-start me-4 mt-8 max-md:pt-2">
      <div class="text-base-content/50 text-sm font-normal">2 day’s ago</div>
    </div>
    <div class="timeline-end ms-4">
      <div class="card">
        <div class="card-body gap-4">
          <h5 class="card-title text-lg">Johnson shared NextJS project</h5>
          <p>
            The project organization's structure and process are meticulously crafted to align with both corporate and
            project goals. Key components include planning, execution, monitoring, controlling, resource allocation,
            risk management, and stakeholder engagement.
          </p>
          <div class="card-actions">
            <button class="btn btn-soft btn-sm btn-secondary">
              <span class="icon-[tabler--file-type-xls] text-success max-sm:hidden"></span>
              progress-report.xls
            </button>
          </div>
            <div class="flex w-full items-center gap-2">
              <div class="progress" role="progressbar" aria-label="Progressbar" aria-valuenow="34" aria-valuemin="0" aria-valuemax="100">
                <div class="progress-bar progress-primary w-[34%]"></div>
              </div>
              <span class="text-sm font-medium">34%</span>
            </div>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 5-->
</ul>
```

<!--  Activity log  -->

### Activity log

Use the provided example for timeline as activity log.

```html
<ul class="timeline timeline-vertical timeline-compact w-full">
  <!-- timeline item 1-->
  <li>
    <hr />
    <div class="timeline-middle h-12">
      <div class="avatar">
        <div class="size-8 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
        </div>
      </div>
    </div>
    <div class="timeline-end w-full">
      <div class="border-base-content/25 flex w-full flex-wrap items-center justify-between gap-2 rounded-lg border p-3" >
        <p>
          John added
          <a class="link link-info link-hover font-medium">@verreyne</a>
          to
          <span class="badge badge-soft badge-secondary badge-sm rounded-full">FlyonUI</span>
          Group as a member
        </p>
        <div class="text-base-content/50 text-nowrap text-sm">just now</div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 1-->
  <!-- timeline item 2-->
  <li>
    <hr />
    <div class="timeline-middle bg-base-100 row-start-1 h-12">
      <div class="avatar">
        <div class="size-8 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
        </div>
      </div>
    </div>
    <div class="timeline-end mt-6 w-full">
      <div class="border-base-content/25 rounded-lg border p-3">
        <div class="mb-3 flex w-full flex-wrap items-center justify-between gap-2">
          <p>
            Casey commented on
            <span class="text-base-content font-medium">FlyonUI</span>
            design
          </p>
          <span class="text-base-content/50 text-nowrap text-sm">3 hours ago</span>
        </div>
        <div class="border-base-content/25 bg-base-200/50 rounded-lg border p-3 text-xs font-normal italic">
          Hello everyone! I'm excited to inform you about an upcoming webinar hosted by FlyonUI core team, focusing on the
          topic of effectively measuring your design system. This webinar marks the second session of our new series on
          #FlyonDesign discussions, where we delve into various aspects of design systems. In this session, we'll be
          exploring the topic of Measurement.
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 2-->
  <!-- timeline item 3-->
  <li>
    <hr />
    <div class="timeline-middle h-12">
      <div class="avatar">
        <div class="size-8 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-8.png" alt="User Avatar" />
        </div>
      </div>
    </div>
    <div class="timeline-end mt-6 w-full">
      <div class="border-base-content/25 flex w-full flex-wrap items-center justify-between gap-2 rounded-lg border p-3" >
        <p>
          Anna has changed
          <a class="link link-primary link-hover font-medium">Documentation</a>
          layout task status from
          <span class="badge badge-outline badge-secondary badge-sm rounded-full">Ongoing</span>
          to
          <span class="badge badge-outline badge-success badge-sm rounded-full">Finished</span>
        </p>
        <div class="text-base-content/50 text-nowrap text-sm">1 day ago</div>
      </div>
    </div>
    <hr />
  </li>
  <!-- timeline item 3-->
  <!-- timeline item 4-->
  <li>
    <hr />
    <div class="timeline-middle h-12">
      <div class="avatar">
        <div class="size-8 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-7.png" alt="User Avatar" />
        </div>
      </div>
    </div>
    <div class="timeline-end mt-6 w-full">
      <div class="border-base-content/25 flex w-full flex-wrap items-center justify-between gap-2 rounded-lg border p-3" >
        <p>
          James has changed
          <a class="link link-primary link-hover font-medium">Forums</a>
          page task status from
          <span class="badge badge-outline badge-secondary badge-sm rounded-full">pending</span>
          to
          <span class="badge badge-outline badge-primary badge-sm rounded-full">Started</span>
        </p>
        <div class="text-base-content/50 text-nowrap text-sm">1 month ago</div>
      </div>
    </div>
    <hr />
  </li>
  <!-- timeline item 4-->
  <!-- timeline item 5-->
  <li>
    <hr />
    <div class="timeline-middle h-12">
      <div class="avatar">
        <div class="size-8 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Avatar" />
        </div>
      </div>
    </div>
    <div class="timeline-end mt-6 w-full">
      <div class="border-base-content/25 flex w-full flex-wrap items-center justify-between gap-2 rounded-lg border p-3" >
        <p>
          Adam has initiated branch project
          <a class="link link-primary link-hover font-medium">FlyonUI</a>
          pro with
          <a class="link link-info link-hover font-medium">@Casey</a>
        </p>
        <div class="text-base-content/50 text-nowrap text-sm">3 months ago</div>
      </div>
    </div>
    <hr />
  </li>
  <!-- timeline item 5-->
</ul>
```

<!--  Collapsed  -->

### Collapsed

Use the provided example for timeline with last item collapsed.

> **Info:** Refer [collapse](components/collapse/) plugin for more details.
```html
<ul class="timeline timeline-snap-icon timeline-compact timeline-vertical w-full">
  <span class="text-sm">April 1, 2024</span>
  <!-- timeline item 1-->
  <li>
    <div class="timeline-middle">
      <span class="bg-primary/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-primary size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">12 Invoices have been paid</div>
      <p class="mb-2">Invoices have been paid to the company</p>
      <button class="btn btn-sm btn-soft btn-secondary">
        <span class="icon-[tabler--file-type-pdf] text-error"></span>
        invoices.pdf
      </button>
    </div>
    <hr />
  </li>
  <!-- /timeline item 1-->
  <span class="mt-2 text-sm">March 31, 2024</span>
  <!-- timeline item 2-->
  <li>
    <div class="timeline-middle">
      <span class="bg-success/20 flex size-4.5 items-center justify-center rounded-full">
        <span class="badge badge-success size-3 rounded-full p-0"></span>
      </span>
    </div>
    <div class="timeline-end ms-2 m-3 w-full rounded-lg">
      <div class="text-base-content pt-0.5 mb-3 font-medium">Client meeting</div>
      <p class="mb-2">Project meeting with john @10:15am</p>
      <div class="flex gap-2">
        <div class="avatar">
          <div class="size-8 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
          </div>
        </div>
        <div class="text-sm">
          <p class="font-medium">Lester McCarthy (Client)</p>
          <p>CEO of ThemeSelection</p>
        </div>
      </div>
    </div>
    <hr />
  </li>
  <!-- /timeline item 2-->
  <!-- timeline item 3-->
  <!-- Collapsed timeline trigger text -->
  <button class="collapse-toggle text-primary collapse-open:text-base-content/80 -mb-2 mt-2 flex items-center text-sm" id="timeline-collapse-content" data-collapse="#timeline-collapse" >
    March 31, 2024
    <span class="collapse-open:rotate-180 icon-[tabler--caret-down-filled] ms-0.5"></span>
  </button>
  <!-- /Collapsed timeline trigger text -->
  <!-- Collapsed timeline target content -->
  <ul id="timeline-collapse" class="timeline timeline-snap-icon timeline-compact timeline-vertical collapse hidden w-full overflow-hidden transition-all duration-300 ease-in-out" aria-labelledby="timeline-collapse-content" >
    <li>
      <div class="timeline-middle">
        <span class="bg-info/20 flex size-4.5 items-center justify-center rounded-full">
          <span class="badge badge-info size-3 rounded-full p-0"></span>
        </span>
      </div>
      <div class="timeline-end ms-2 m-3 w-full rounded-lg">
        <div class="text-base-content pt-0.5 mb-3 font-medium">Create a new project for client</div>
        <p class="mb-2">6 team members in a project</p>
        <div class="avatar-group pull-up -space-x-4">
          <div class="avatar">
            <div class="w-8">
              <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Avatar" />
            </div>
          </div>
          <div class="avatar">
            <div class="w-8">
              <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Avatar" />
            </div>
          </div>
          <div class="avatar">
            <div class="w-8">
              <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Avatar" />
            </div>
          </div>
          <div class="avatar avatar-placeholder">
            <div class="bg-neutral text-neutral-content w-8">
              <span>+3</span>
            </div>
          </div>
        </div>
      </div>
      <hr />
    </li>
  </ul>
  <!-- /Collapsed timeline target content -->
  <!-- /timeline item 3-->
</ul>
```
