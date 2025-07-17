# Menu

The menu component presents a vertical or horizontal list of links for easy navigation within the application or website.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| menu | component | Base class for menu container. |
| menu-title | part | Base class for menu title. |
| menu-disabled | state | Makes menu item (`li`) disabled. |
| menu-active | state | Makes element inside menu item (`li`) active. |
| menu-xs | size | Extra small size. |
| menu-sm | size | Small size. |
| menu-md | size | Medium(default) size. |
| menu-lg | size | Large size. |
| menu-xl | size | Extra-Large size. |
| menu-vertical | direction | Vertical menu (default). |
| menu-horizontal | direction | Horizontal menu. |


<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Below example shows default menu component.

```html
<ul class="menu">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
```

<!-------------------- Variants -------------------->

## Variants

<!-- Icon menu -->

### Icon menu

Below example shows menu with icons.

```html
<ul class="menu">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--user] size-5"></span>
      Account
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--message] size-5"></span>
      Notifications
    </a>
  </li>
</ul>
```

<!-- With icons only -->

### With icons only

Below example shows menu with icons only.

```html
<ul class="menu">
  <li>
    <a href="#" aria-label="Home Link"><span class="icon-[tabler--home] size-5"></span></a>
  </li>
  <li>
    <a href="#" aria-label="User Link"><span class="icon-[tabler--user] size-5"></span></a>
  </li>
  <li>
    <a href="#" aria-label="Message Link"><span class="icon-[tabler--message] size-5"></span></a>
  </li>
</ul>
```

<!-- With icons only (horizontal) -->

### With icons only (horizontal)

Use the responsive class `menu-horizontal` with the component class `menu` for a horizontal menu.

Below example shows menu with icons only.

```html
<ul class="menu menu-horizontal">
  <li>
    <a href="#" aria-label="Home Link"><span class="icon-[tabler--home] size-5"></span></a>
  </li>
  <li>
    <a href="#" aria-label="User Link"><span class="icon-[tabler--user] size-5"></span></a>
  </li>
  <li>
    <a href="#" aria-label="Message Link"><span class="icon-[tabler--message] size-5"></span></a>
  </li>
</ul>
```

<!-- With tooltip -->

### With tooltip

Below example shows menu with tooltip.

```html
<ul class="menu">
  <li class="tooltip [--placement:right]">
    <a href="#" class="tooltip-toggle" aria-label="Home Link"><span class="icon-[tabler--home] size-5"></span></a>
    <span class="tooltip-content tooltip-shown:opacity-100 tooltip-shown:visible" role="tooltip">
      <span class="tooltip-body">Home</span>
    </span>
  </li>
  <li class="tooltip [--placement:right]">
    <a href="#" class="tooltip-toggle" aria-label="User Link"><span class="icon-[tabler--user] size-5"></span></a>
    <span class="tooltip-content tooltip-shown:opacity-100 tooltip-shown:visible" role="tooltip">
      <span class="tooltip-body">Account</span>
    </span>
  </li>
  <li class="tooltip [--placement:right]">
    <a href="#" class="tooltip-toggle" aria-label="Message Link"><span class="icon-[tabler--message] size-5"></span></a>
    <span class="tooltip-content tooltip-shown:opacity-100 tooltip-shown:visible" role="tooltip">
      <span class="tooltip-body">Notifications</span>
    </span>
  </li>
</ul>
```

<!-- With disabled items -->

### With disabled items

Below example shows menu with disabled items.

```html
<ul class="menu">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>
  <li class="menu-disabled">
    <a href="#">
      <span class="icon-[tabler--lock] size-5"></span>
      Security
    </a>
  </li>
</ul>
```

<!-- With badges -->

### With badges

Below example shows menu with badges.

```html
<ul class="menu lg:menu-horizontal">
  <li>
    <a href="#">
      <span class="icon-[tabler--mail] size-5"></span>
      Inbox
      <span class="badge badge-sm badge-primary">1K+</span>
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--info-circle] size-5"></span>
      Updates
      <span class="badge badge-sm badge-warning">NEW</span>
    </a>
  </li>
  <li>
    <a href="#">

      Status
      <span class="badge badge-success size-3 p-0"></span>
    </a>

  </li>
</ul>
```

<!-- With item -->

### With item

Below example shows menu with item.

```html
<ul class="menu">
  <li>
    <a href="#" class="menu-active">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--user] size-5"></span>
      Account
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--message] size-5"></span>
      Notifications
    </a>
  </li>
</ul>
```

<!-------------------- Sizes -------------------->

## Sizes

<!-- Basic sizes -->

### Basic sizes

Utilize the responsive class `menu-{size}` where `size = xs|sm|md|lg|xl` to render menus of varying sizes.

The following example demonstrates menus with different sizes.

```html
<ul class="menu menu-xs w-fit">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
<ul class="menu menu-sm w-fit">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
<ul class="menu menu-md w-fit">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
<ul class="menu menu-lg w-fit">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
<ul class="menu menu-xl w-fit">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Simple -->

### Simple

Below example shows simple menu without rounded borders & padding.

```html
<ul class="menu rounded-none p-0 [&_li>*]:rounded-none">
  <li><a href="#">Home</a></li>
  <li><a href="#">Account</a></li>
  <li><a href="#">Notifications</a></li>
</ul>
```

<!-- With title -->

### With title

Below example shows menu with title.

```html
<ul class="menu">
  <li class="menu-title">Apps</li>
  <li>
    <a href="#">
      <span class="icon-[tabler--message] size-5"></span>
      Chat
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--calendar] size-5"></span>
      Calendar
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--book] size-5"></span>
      Academy
    </a>
  </li>
</ul>
```

<!-- With title as parent -->

### With title as parent

Below example shows menu with title as parent.

```html
<ul class="menu">
  <li>
    <p class="menu-title">Apps</p>
    <ul>
      <li>
        <a href="#">
          <span class="icon-[tabler--message] size-5"></span>
          Chat
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--calendar] size-5"></span>
          Calendar
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--book] size-5"></span>
          Academy
        </a>
      </li>
    </ul>
  </li>
</ul>
```

<!-- With sub-menus -->

### With sub-menus

Below example shows menu with sub-menus.

```html
<ul class="menu">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--apps] size-5"></span>
      Apps
    </a>
    <ul class="menu">
      <li>
        <a href="#">
          <span class="icon-[tabler--message] size-5"></span>
          Chat
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--calendar] size-5"></span>
          Calendar
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--book] size-5"></span>
          Academy
        </a>
        <ul class="menu">
          <li>
            <a href="#">
              <span class="icon-[tabler--books] size-5"></span>
              Courses
            </a>
          </li>
          <li>
            <a href="#">
              <span class="icon-[tabler--list-details] size-5"></span>
              Course details
            </a>
          </li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>
</ul>
```

<!-- Collapsible sub-menus -->

### Collapsible sub-menus

Below example shows menu with collapsible sub-menus.

<!-- With Collapse -->
#### With Collapse

This example uses collapse to achieve this. Refer to the [Collapse](components/collapse/) component for more details.


```html
<ul class="menu w-64 space-y-0.5">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li class="space-y-0.5">
    <a class="collapse-toggle collapse-open:bg-base-content/10 open" id="menu-app" data-collapse="#menu-app-collapse">
      <span class="icon-[tabler--apps] size-5"></span>
      Apps
      <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4 transition-all duration-300"></span>
    </a>
    <ul id="menu-app-collapse" class="open collapse w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app" >
      <li>
        <a href="#">
          <span class="icon-[tabler--message] size-5"></span>
          Chat
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--calendar] size-5"></span>
          Calendar
        </a>
      </li>
      <li class="space-y-0.5">
        <a class="collapse-toggle collapse-open:bg-base-content/10 open" id="sub-menu-academy" data-collapse="#sub-menu-academy-collapse" >
          <span class="icon-[tabler--book] size-5"></span>
          Academy
          <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4"></span>
        </a>
        <ul id="sub-menu-academy-collapse" class="open collapse w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy" >
          <li>
            <a href="#">
              <span class="icon-[tabler--books] size-5"></span>
              Courses
            </a>
          </li>
          <li>
            <a href="#">
              <span class="icon-[tabler--list-details] size-5"></span>
              Course details
            </a>
          </li>
          <li class="space-y-0.5">
            <a class="collapse-toggle collapse-open:bg-base-content/10 open" id="sub-menu-academy-stats" data-collapse="#sub-menu-academy-stats-collapse" >
              <span class="icon-[tabler--chart-bar] size-5"></span>
              Stats
              <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4"></span>
            </a>
            <ul id="sub-menu-academy-stats-collapse" class="open collapse w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-stats" >
              <li>
                <a href="#">
                  <span class="icon-[tabler--chart-donut] size-5"></span>
                  Goals
                </a>
              </li>
            </ul>
          </li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>
</ul>
```


<!-- With accordion -->
{{< headname level="4" badge-text="new">}} With accordion {{< /headname >}}

This example uses accordion to achieve this. Refer to the [Accordion](components/accordion/) component for more details.

```html
<ul class="menu accordion w-64 space-y-0.5">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>

  <!-- First Accordion Item -->
  <li class="accordion-item active space-y-0.5" id="menu-app-1">
    <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="menu-app-collapse-1" aria-expanded="true" >
      <span class="icon-[tabler--apps] size-5"></span>
      <span class="grow">Apps</span>
      <span class="icon-[tabler--chevron-down] size-4 transition-all duration-300"></span>
    </button>
    <div id="menu-app-collapse-1" class="accordion-content w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app-1" role="region" >
      <ul class="accordion space-y-0.5">
        <li>
          <a href="#">
            <span class="icon-[tabler--message] size-5"></span>
            Chat
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--calendar] size-5"></span>
            Calendar
          </a>
        </li>
        <!-- Nested Accordion Item (Academy) -->
        <li class="accordion-item space-y-0.5" id="sub-menu-academy-1">
          <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-academy-collapse-1" aria-expanded="false" >
            <span class="icon-[tabler--book] size-5"></span>
            <span class="grow">Academy</span>
            <span class="icon-[tabler--chevron-down] size-4"></span>
          </button>
          <div id="sub-menu-academy-collapse-1" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-1" role="region" >
            <ul class="accordion space-y-0.5">
              <li>
                <a href="#">
                  <span class="icon-[tabler--books] size-5"></span>
                  Courses
                </a>
              </li>
              <li>
                <a href="#">
                  <span class="icon-[tabler--list-details] size-5"></span>
                  Course details
                </a>
              </li>
              <!-- Nested Accordion Item (Stats) -->
              <li class="accordion-item space-y-0.5" id="sub-menu-academy-stats-1">
                <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-academy-stats-collapse-1" aria-expanded="false" > <span class="icon-[tabler--chart-bar] size-5"></span>
                  <span class="grow">Stats</span>
                  <span class="icon-[tabler--chevron-down] size-4"></span>
                </button>
                <div id="sub-menu-academy-stats-collapse-1" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-stats-1" role="region" >
                  <ul class="space-y-0.5">
                    <li>
                      <a href="#">
                        <span class="icon-[tabler--chart-donut] size-5"></span>
                        Goals
                      </a>
                    </li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </li>

  <!-- Settings -->
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>

  <!-- Second Accordion Item (Updated) -->
  <li class="accordion-item space-y-0.5" id="menu-app-2">
    <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="menu-app-collapse-2" aria-expanded="false" >
      <span class="icon-[tabler--apps] size-5"></span>
      <span class="grow">More Apps</span>
      <span class="icon-[tabler--chevron-down] size-4 transition-all duration-300"></span>
    </button>
    <div id="menu-app-collapse-2" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app-2" role="region" >
      <ul class="accordion space-y-0.5">
        <li>
          <a href="#">
            <span class="icon-[tabler--clock] size-5"></span>
            Clock
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--file-text] size-5"></span>
            Files
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--camera] size-5"></span>
            Camera
          </a>
        </li>
        <!-- Nested Accordion Item (Reports) -->
        <li class="accordion-item space-y-0.5" id="sub-menu-reports-1">
          <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-reports-collapse-1" aria-expanded="false" >
            <span class="icon-[tabler--clipboard-list] size-5"></span>
            <span class="grow">Reports</span>
            <span class="icon-[tabler--chevron-down] size-4"></span>
          </button>
          <div id="sub-menu-reports-collapse-1" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-reports-1" role="region" >
            <ul class="space-y-0.5">
              <li>
                <a href="#">
                  <span class="icon-[tabler--clipboard-check] size-5"></span>
                  Daily Report
                </a>
              </li>
              <li>
                <a href="#">
                  <span class="icon-[tabler--clipboard-x] size-5"></span>
                  Weekly Report
                </a>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </li>
</ul>
```

<!-- With accordion always open -->
{{< headname level="4" badge-text="new" >}} With accordion always open {{< /headname >}}

This example uses accordion always open to achieve this. Refer to the [Accordion Always open](components/accordion/#always-open) component for more details.

```html
<ul class="menu accordion w-64 space-y-0.5" data-accordion-always-open>
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>

  <!-- First Accordion Item -->
  <li class="accordion-item active space-y-0.5" id="menu-app-1-unique">
    <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="menu-app-collapse-1-unique" aria-expanded="true">
      <span class="icon-[tabler--apps] size-5"></span>
      <span class="grow">Apps</span>
      <span class="icon-[tabler--chevron-down] size-4 transition-all duration-300"></span>
    </button>
    <div id="menu-app-collapse-1-unique" class="accordion-content w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app-1-unique" role="region">
      <ul class="accordion space-y-0.5" data-accordion-always-open>
        <li>
          <a href="#">
            <span class="icon-[tabler--message] size-5"></span>
            Chat
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--calendar] size-5"></span>
            Calendar
          </a>
        </li>
        <!-- Nested Accordion Item (Academy) -->
        <li class="accordion-item space-y-0.5" id="sub-menu-academy-1-unique">
          <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-academy-collapse-1-unique" aria-expanded="false">
            <span class="icon-[tabler--book] size-5"></span>
            <span class="grow">Academy</span>
            <span class="icon-[tabler--chevron-down] size-4"></span>
          </button>
          <div id="sub-menu-academy-collapse-1-unique" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-1-unique" role="region">
            <ul class="accordion space-y-0.5" data-accordion-always-open>
              <li>
                <a href="#">
                  <span class="icon-[tabler--books] size-5"></span>
                  Courses
                </a>
              </li>
              <li>
                <a href="#">
                  <span class="icon-[tabler--list-details] size-5"></span>
                  Course details
                </a>
              </li>
              <!-- Nested Accordion Item (Stats) -->
              <li class="accordion-item space-y-0.5" id="sub-menu-academy-stats-1-unique">
                <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-academy-stats-collapse-1-unique" aria-expanded="false">
                  <span class="icon-[tabler--chart-bar] size-5"></span>
                  <span class="grow">Stats</span>
                  <span class="icon-[tabler--chevron-down] size-4"></span>
                </button>
                <div id="sub-menu-academy-stats-collapse-1-unique" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-stats-1-unique" role="region">
                  <ul class="space-y-0.5">
                    <li>
                      <a href="#">
                        <span class="icon-[tabler--chart-donut] size-5"></span>
                        Goals
                      </a>
                    </li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </li>

  <!-- Settings -->
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>

  <!-- Second Accordion Item (Updated) -->
  <li class="accordion-item space-y-0.5" id="menu-app-2-unique">
    <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="menu-app-collapse-2-unique" aria-expanded="false">
      <span class="icon-[tabler--apps] size-5"></span>
      <span class="grow">More Apps</span>
      <span class="icon-[tabler--chevron-down] size-4 transition-all duration-300"></span>
    </button>
    <div id="menu-app-collapse-2-unique" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app-2-unique" role="region">
      <ul class="accordion space-y-0.5" data-accordion-always-open>
        <li>
          <a href="#">
            <span class="icon-[tabler--clock] size-5"></span>
            Clock
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--file-text] size-5"></span>
            Files
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--camera] size-5"></span>
            Camera
          </a>
        </li>
        <!-- Nested Accordion Item (Reports) -->
        <li class="accordion-item space-y-0.5" id="sub-menu-reports-1-unique">
          <button class="accordion-toggle rounded-field inline-flex items-center gap-x-4 px-4 py-2.5 text-start text-base font-normal" aria-controls="sub-menu-reports-collapse-1-unique" aria-expanded="false">
            <span class="icon-[tabler--clipboard-list] size-5"></span>
            <span class="grow">Reports</span>
            <span class="icon-[tabler--chevron-down] size-4"></span>
          </button>
          <div id="sub-menu-reports-collapse-1-unique" class="accordion-content hidden w-full space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-reports-1-unique" role="region">
            <ul class="space-y-0.5">
              <li>
                <a href="#">
                  <span class="icon-[tabler--clipboard-check] size-5"></span>
                  Daily Report
                </a>
              </li>
              <li>
                <a href="#">
                  <span class="icon-[tabler--clipboard-x] size-5"></span>
                  Weekly Report
                </a>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </li>
</ul>
```

<!-- With horizontal sub-menu -->

### With horizontal sub-menu

Below example shows horizontal menu with sub-menu.

```html
<ul class="menu sm:menu-horizontal">
  <li>
    <a href="#">
      <span class="icon-[tabler--home] size-5"></span>
      Home
    </a>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--apps] size-5"></span>
      Apps
    </a>
    <ul class="menu">
      <li>
        <a href="#">
          <span class="icon-[tabler--message] size-5"></span>
          Chat
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--calendar] size-5"></span>
          Calendar
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--book] size-5"></span>
          Academy
        </a>
      </li>
    </ul>
  </li>
  <li>
    <a href="#">
      <span class="icon-[tabler--settings] size-5"></span>
      Settings
    </a>
  </li>
</ul>
```

<!-- Mega menu with sub-menu -->

### Mega menu with sub-menu

Below example shows mega menu with sub-menu.

```html
<ul class="menu sm:menu-horizontal">
  <li>
    <span class="menu-title">Services</span>
    <ul class="menu">
      <li><a href="#">Design Solutions</a></li>
      <li><a href="#">Software Development</a></li>
      <li><a href="#">Web Hosting</a></li>
      <li><a href="#">Domain Registration</a></li>
    </ul>
  </li>
  <li>
    <span class="menu-title">Corporate Solutions</span>
    <ul class="menu">
      <li><a href="#">CRM</a></li>
      <li><a href="#">Management Solutions</a></li>
      <li><a href="#">Security Services</a></li>
      <li><a href="#">Consulting Services</a></li>
    </ul>
  </li>
  <li>
    <span class="menu-title">Product Offerings</span>
    <ul class="menu">
      <li><a href="#">UI Kits</a></li>
      <li><a href="#">Component Library</a></li>
      <li><a href="#">WordPress Plugins</a></li>
      <li>
        <span class="menu-title">Open Source Projects</span>
        <ul class="menu">
          <li><a href="#">Authentication System</a></li>
          <li><a href="#">FlyonUI Theme</a></li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <span class="menu-title">Company</span>
    <ul class="menu">
      <li><a href="#">About us</a></li>
      <li><a href="#">Contact us</a></li>
      <li><a href="#">Privacy policy</a></li>
      <li><a href="#">Careers</a></li>
    </ul>
  </li>
</ul>
```

<!-- Menu with dropdown -->

### Menu with dropdown

Below example shows menu with dropdown.

```html
<ul class="menu menu-horizontal space-x-0.5">
  <li><a href="#">Home</a></li>
  <li><a href="#">Services</a></li>
  <li class="dropdown relative inline-flex [--auto-close:inside] [--offset:9] [--placement:bottom-end]">
    <button id="dropdown-end" type="button" class="dropdown-toggle dropdown-open:bg-base-content/10 dropdown-open:text-base-content max-sm:px-2" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
      Products
      <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
    </button>
    <ul class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-end">
      <li><a class="dropdown-item" href="#">UI kits</a></li>
      <li><a class="dropdown-item" href="#">Templates</a></li>
      <li><a class="dropdown-item" href="#">Component library</a></li>
      <hr class="border-base-content/25 -mx-2 my-3" />
      <li><a class="dropdown-item" href="#">Figma designs</a></li>
    </ul>
  </li>
</ul>
```
