# Sidebar

Utilize a sidebar component on both sides of the page to display a list of menu items, including multi-level navigation options, for easy website navigation.

> **Info:** This example demonstrates the use of multiple components, including the [Drawer](overlays/drawer/), [Menu](navigations/menu/),  [Collapse](components/collapse/), [Accordion](components/accordion/) and [Dropdown](overlays/dropdown/) components, which implement overall functionality for the sidebar features.

<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Create a responsive sidebar menu that contains a list of items, each with an associated icon and label. Utilize the `[--auto-close:*]` responsive value, such as `sm`, `md`, `lg`, `xl`, or `2xl`, to automatically close the overlay based on the screen size.

> **Warning:** Please remove `sm:z-0` and `sm:absolute`, as these were applied for a specific condition in our case. Since some styles are conditional, kindly remove any unnecessary classes.

```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="default-sidebar" data-overlay="#default-sidebar" >
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="default-sidebar" class="overlay [--auto-close:sm] sm:shadow-none overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 sm:absolute sm:z-0 sm:flex sm:translate-x-0" role="dialog" tabindex="-1" >
  <div class="drawer-body px-2 pt-4">
    <ul class="menu p-0">
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
      <li>
        <a href="#">
          <span class="icon-[tabler--mail] size-5"></span>
          Email
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
          <span class="icon-[tabler--shopping-bag] size-5"></span>
          Product
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
    </ul>
  </div>
</aside>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Multiple level with separator -->

### Multiple level with separator

Use this example to create a multi-level sidebar by utilizing the collapse feature with the menu for collapsible items, and the divider component to create separators.

> **Warning:** Please remove `sm:z-0` and `sm:absolute`, as these were applied for a specific condition in our case. Since some styles are conditional, kindly remove any unnecessary classes.

```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="multilevel-with-separator" data-overlay="#multilevel-with-separator" >
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="multilevel-with-separator" class="overlay [--auto-close:sm] overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 sm:absolute sm:z-0 sm:flex sm:translate-x-0 sm:shadow-none" tabindex="-1" >
  <div class="drawer-body px-2 pt-4">
    <ul class="menu space-y-0.5 p-0">
      <li>
        <a href="#">
          <span class="icon-[tabler--home] size-5"></span>
          Home
        </a>
      </li>
      <li class="space-y-0.5">
        <a class="collapse-toggle collapse-open:bg-base-content/10" id="menu-app" data-collapse="#menu-app-collapse">
          <span class="icon-[tabler--apps] size-5"></span>
          Apps
          <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4 transition-all duration-300"></span>
        </a>
        <ul id="menu-app-collapse" class="collapse hidden w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="menu-app" >
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
            <a class="collapse-toggle collapse-open:bg-base-content/10" id="sub-menu-academy" data-collapse="#sub-menu-academy-collapse" >
              <span class="icon-[tabler--book] size-5"></span>
              Academy
              <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4"></span>
            </a>
            <ul id="sub-menu-academy-collapse" class="collapse hidden w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy" >
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
                <a class="collapse-toggle collapse-open:bg-base-content/10" id="sub-menu-academy-stats" data-collapse="#sub-menu-academy-stats-collapse" >
                  <span class="icon-[tabler--chart-bar] size-5"></span>
                  Stats
                  <span class="icon-[tabler--chevron-down] collapse-open:rotate-180 size-4"></span>
                </a>
                <ul id="sub-menu-academy-stats-collapse" class="collapse hidden w-auto space-y-0.5 overflow-hidden transition-[height] duration-300" aria-labelledby="sub-menu-academy-stats" >
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
      <div class="divider text-base-content/50 py-6 after:border-0">Account</div>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
      <div class="divider text-base-content/50 py-6 after:border-0">Miscellaneous</div>
      <li>
        <a href="#">
          <span class="icon-[tabler--users-group] size-5"></span>
          Support
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--files] size-5"></span>
          Documentation
        </a>
      </li>
    </ul>
  </div>
</aside>
```

<!-- CTA button -->

### CTA button

Use this example to incorporate a CTA button within the sidebar, guiding users to visit the dedicated page.

> **Warning:** Please remove `sm:z-0` and `sm:absolute`, as these were applied for a specific condition in our case. Since some styles are conditional, kindly remove any unnecessary classes.

```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="cta-sidebar" data-overlay="#cta-sidebar" >
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="cta-sidebar" class="overlay [--auto-close:sm] overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 sm:absolute sm:z-0 sm:flex sm:translate-x-0 sm:shadow-none" role="dialog" tabindex="-1" >
  <div class="drawer-body px-2 py-4">
    <ul class="menu p-0">
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
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
    </ul>
    <div class="bg-base-200/30 border-base-content/10 mt-4 rounded-md border p-3">
      <div class="avatar avatar-placeholder">
        <div class="bg-neutral text-neutral-content w-10 rounded-full">
          <span class="icon-[tabler--crown] size-6 shrink-0"></span>
        </div>
      </div>
      <h5 class="text-base-content mt-4 text-lg font-semibold">Upgrade to Pro</h5>
      <p class="text-base-content/80 text-xs">Reminder, extra projects, advanced search and more</p>
      <button class="btn btn-primary btn-block mt-2">Upgrade Now</button>
    </div>
  </div>
</aside>
```

<!-- Logo branding -->

### Logo branding

Display your brand's logo and link it back to the homepage at the top of the sidebar.

> **Warning:** Please remove `sm:z-0` and `sm:absolute`, as these were applied for a specific condition in our case. Since some styles are conditional, kindly remove any unnecessary classes.

```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="logo-sidebar" data-overlay="#logo-sidebar" >
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="logo-sidebar" class="overlay [--auto-close:sm] sm:shadow-none overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 sm:absolute sm:z-0 sm:flex sm:translate-x-0" role="dialog" tabindex="-1" >
  <div class="drawer-header">
    <div class="flex items-center gap-3">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z" fill="var(--color-primary)"/></svg>
      <h3 class="drawer-title text-xl font-semibold">FlyonUI</h3>
    </div>
  </div>
  <div class="drawer-body px-2">
    <ul class="menu p-0">
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
      <li>
        <a href="#">
          <span class="icon-[tabler--mail] size-5"></span>
          Email
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
          <span class="icon-[tabler--shopping-bag] size-5"></span>
          Product
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
    </ul>
  </div>
</aside>
```

<!-- With navbar -->

### With navbar

Use this example to demonstrate a layout that includes both a navbar and a sidebar for your web application.

> **Warning:** Please remove `sm:z-0` and `sm:absolute`, as these were applied for a specific condition in our case. Since some styles are conditional, kindly remove any unnecessary classes.

```html
<nav class="navbar bg-base-100 max-sm:rounded-box max-sm:shadow-sm sm:border-b border-base-content/25 sm:z-1 relative">
  <button type="button" class="btn btn-text max-sm:btn-square sm:hidden me-2" aria-haspopup="dialog" aria-expanded="false" aria-controls="with-navbar-sidebar" data-overlay="#with-navbar-sidebar" >
    <span class="icon-[tabler--menu-2] size-5"></span>
  </button>
  <div class="flex flex-1 items-center">
    <a class="link text-base-content link-neutral text-xl font-semibold no-underline" href="#">
      FlyonUI
    </a>
  </div>
  <div class="navbar-end flex items-center gap-4">
    <div class="dropdown relative inline-flex [--auto-close:inside] [--offset:8] [--placement:bottom-end]">
      <button id="dropdown-scrollable" type="button" class="dropdown-toggle btn btn-text btn-circle dropdown-open:bg-base-content/10 size-10" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
        <div class="indicator">
          <span class="indicator-item bg-error size-2 rounded-full"></span>
          <span class="icon-[tabler--bell] text-base-content size-5.5"></span>
        </div>
      </button>
      <div class="dropdown-menu dropdown-open:opacity-100 hidden" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-scrollable">
        <div class="dropdown-header justify-center">
          <h6 class="text-base-content text-base">Notifications</h6>
        </div>
        <div class="overflow-y-auto overflow-x-auto text-base-content/80 max-h-56 overflow-auto max-md:max-w-60">
          <div class="dropdown-item">
            <div class="avatar avatar-away-bottom">
              <div class="w-10 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="avatar 1" />
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">Charles Franklin</h6>
              <small class="text-base-content/50 truncate">Accepted your connection</small>
            </div>
          </div>
          <div class="dropdown-item">
            <div class="avatar">
              <div class="w-10 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="avatar 2" />
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">Martian added moved Charts & Maps task to the done board.</h6>
              <small class="text-base-content/50 truncate">Today 10:00 AM</small>
            </div>
          </div>
          <div class="dropdown-item">
            <div class="avatar avatar-online-bottom">
              <div class="w-10 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-8.png" alt="avatar 8" />
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">New Message</h6>
              <small class="text-base-content/50 truncate">You have new message from Natalie</small>
            </div>
          </div>
          <div class="dropdown-item">
            <div class="avatar avatar-placeholder">
              <div class="bg-neutral text-neutral-content w-10 rounded-full p-2">
                <span class="icon-[tabler--user] size-full"></span>
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">Application has been approved 🚀</h6>
              <small class="text-base-content/50 text-wrap">Your ABC project application has been approved.</small>
            </div>
          </div>
          <div class="dropdown-item">
            <div class="avatar">
              <div class="w-10 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-10.png" alt="avatar 10" />
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">New message from Jane</h6>
              <small class="text-base-content/50 text-wrap">Your have new message from Jane</small>
            </div>
          </div>
          <div class="dropdown-item">
            <div class="avatar">
              <div class="w-10 rounded-full">
                <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="avatar 3" />
              </div>
            </div>
            <div class="w-60">
              <h6 class="truncate text-base">Barry Commented on App review task.</h6>
              <small class="text-base-content/50 truncate">Today 8:32 AM</small>
            </div>
          </div>
        </div>
        <a href="#" class="dropdown-footer justify-center gap-1">
          <span class="icon-[tabler--eye] size-4"></span>
          View all
        </a>
      </div>
    </div>
    <div class="dropdown relative inline-flex [--auto-close:inside] [--offset:8] [--placement:bottom-end]">
      <button id="dropdown-scrollable" type="button" class="dropdown-toggle flex items-center" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
        <div class="avatar">
          <div class="size-9.5 rounded-full">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="avatar 1" />
          </div>
        </div>
      </button>
      <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-avatar">
        <li class="dropdown-header gap-2">
          <div class="avatar">
            <div class="w-10 rounded-full">
              <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="avatar" />
            </div>
          </div>
          <div>
            <h6 class="text-base-content text-base font-semibold">John Doe</h6>
            <small class="text-base-content/50">Admin</small>
          </div>
        </li>
        <li>
          <a class="dropdown-item" href="#">
            <span class="icon-[tabler--user]"></span>
            My Profile
          </a>
        </li>
        <li>
          <a class="dropdown-item" href="#">
            <span class="icon-[tabler--settings]"></span>
            Settings
          </a>
        </li>
        <li>
          <a class="dropdown-item" href="#">
            <span class="icon-[tabler--receipt-rupee]"></span>
            Billing
          </a>
        </li>
        <li>
          <a class="dropdown-item" href="#">
            <span class="icon-[tabler--help-triangle]"></span>
            FAQs
          </a>
        </li>
        <li class="dropdown-footer gap-2">
          <a class="btn btn-error btn-soft btn-block" href="#">
            <span class="icon-[tabler--logout]"></span>
            Sign out
          </a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<aside id="with-navbar-sidebar" class="overlay [--auto-close:sm] sm:shadow-none overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 sm:absolute sm:z-0 sm:flex sm:translate-x-0 pt-16" role="dialog" tabindex="-1" >
  <div class="drawer-body px-2 pt-4">
    <ul class="menu p-0">
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
      <li>
        <a href="#">
          <span class="icon-[tabler--mail] size-5"></span>
          Email
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
          <span class="icon-[tabler--shopping-bag] size-5"></span>
          Product
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
    </ul>
  </div>
</aside>
```

<!--  Scoped based Sidebar  -->

### Scoped based Sidebar

This example uses `:backdropParent:` to scope the backdrop within a specific block. By default, the backdrop has a `fixed` class applied. To customize the backdrop styling, you can use the `:backdropClasses` option, which completely overrides all default classes for the backdrop. Alternatively, to add additional classes while retaining the default ones, use the `:backdropExtraClasses` option. For more details about these options, please refer to the [Overlay options.](overlays/modal/#options)


```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="scoped-sidebar" data-overlay="#scoped-sidebar" data-overlay-options='{ "backdropExtraClasses": "!absolute", "backdropParent": "#custom-backdrop-container" }'>
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="scoped-sidebar" class="overlay [--auto-close:sm] sm:shadow-none overlay-open:translate-x-0 drawer drawer-start hidden max-w-64 absolute z-1 sm:flex sm:translate-x-0 [--body-scroll:true]" role="dialog" tabindex="-1">
  <div class="drawer-body px-2 pt-4">
    <ul class="menu p-0">
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
      <li>
        <a href="#">
          <span class="icon-[tabler--mail] size-5"></span>
          Email
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
          <span class="icon-[tabler--shopping-bag] size-5"></span>
          Product
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          Sign In
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          Sign Out
        </a>
      </li>
    </ul>
  </div>
</aside>
<div id="custom-backdrop-container"></div>
```

<!-- Drawer sidebar -->
 
### Drawer sidebar

Use this example to implement drawer as an navigation component that appears when an element is clicked.


> **Info:** You can check out this example on the [Drawer](overlays/drawer/#drawer-with-navigation) component page.

---

> **Info:** Sidebar components are adopted from <a href="https://preline.co/docs/sidebar.html" target="_blank" class="link link-primary font-semibold">Preline UI</a> components using <a href="https://preline.co/plugins.html" target="_blank" class="link link-primary font-semibold">Preline’s</a> unstyled, headless Tailwind plugins to deliver accessible and responsive user interfaces.

<!-- Collapsible sidebar -->
{{< headname level="3" badge-text="new" >}} Collapsible sidebar {{< /headname >}}

This example showcases a sidebar that, when opened, shifts the main page content to the side rather than overlaying it. This method ensures both the sidebar and the main content remain visible, offering a smooth navigation experience.

Apply this 2 classes `overlay-body-open` `overlay-body-open:overflow-hidden` in `body` tag

```html
<aside id="collapsible-sidebar" class="overlay [--body-scroll:true] border-base-content/20 overlay-open:translate-x-0 drawer drawer-start sm:overlay-layout-open:translate-x-0 hidden w-64 border-e [--auto-close:sm] [--is-layout-affect:true] [--opened:lg] sm:absolute sm:z-0 sm:flex sm:shadow-none lg:[--overlay-backdrop:false]" role="dialog" tabindex="-1" >
    <div class="drawer-body px-2 pt-4">
      <ul class="menu p-0">
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
        <li>
          <a href="#">
            <span class="icon-[tabler--mail] size-5"></span>
            Email
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
            <span class="icon-[tabler--shopping-bag] size-5"></span>
            Product
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--login] size-5"></span>
            Sign In
          </a>
        </li>
        <li>
          <a href="#">
            <span class="icon-[tabler--logout-2] size-5"></span>
            Sign Out
          </a>
        </li>
      </ul>
    </div>
  </aside>

  <div class="sm:overlay-layout-open:ps-64 min-h-full bg-base-100 transition-all duration-300">
    <!-- Navigation Toggle -->
    <div class="px-2">
      <button type="button" class="btn btn-text btn-square" aria-haspopup="dialog" aria-expanded="false" aria-controls="collapsible-sidebar" data-overlay="#collapsible-sidebar" >
        <span class="icon-[tabler--menu-2] size-5"></span>
      </button>
    </div>
    <!-- End Navigation Toggle -->
  </div>
```

<!-- Collapsible to mini icon sidebar -->
{{< headname level="3" badge-text="new" >}} Collapsible to mini icon sidebar {{< /headname >}}
On desktop, closing the sidebar triggers a smooth transition into a compact mini-sidebar, ensuring both the sidebar and main content stay visible for a seamless, uninterrupted navigation experience.

The `data-overlay-minifier` attribute from `overlay` is used for the button that controls toggling the drawer between its minified and full-width states.

```html
<button type="button" class="btn btn-text max-sm:btn-square sm:hidden" aria-haspopup="dialog" aria-expanded="false" aria-controls="collapsible-mini-sidebar" data-overlay="#collapsible-mini-sidebar" >
  <span class="icon-[tabler--menu-2] size-5"></span>
</button>

<aside id="collapsible-mini-sidebar" class="overlay [--auto-close:sm] overlay-minified:w-17  sm:shadow-none overlay-open:translate-x-0 drawer drawer-start hidden w-66 sm:absolute sm:z-0 sm:flex sm:translate-x-0 border-e border-base-content/20" role="dialog" tabindex="-1" >

<div class="drawer-header  overlay-minified:px-3.75 py-2 w-full flex items-center justify-between gap-3">
    <h3 class="drawer-title text-xl font-semibold overlay-minified:hidden">FlyonUI</h3>
    <div class="hidden sm:block">
        <!-- Toggle Button -->
        <button type="button" class="btn btn-circle btn-text" aria-haspopup="dialog" aria-expanded="false" aria-controls="collapsible-mini-sidebar" aria-label="Minify navigation" data-overlay-minifier="#collapsible-mini-sidebar">
          <span class="icon-[tabler--menu-2] size-5"></span>
          <span class="sr-only">Navigation Toggle</span>
        </button>
        <!-- End Toggle Button -->
      </div>
  </div> 
  <div class="drawer-body px-2 pt-4">
    <ul class="menu p-0">
      <li>
        <a href="#">
          <span class="icon-[tabler--home] size-5"></span>
          <span class="overlay-minified:hidden">Home</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--user] size-5"></span>
          <span class="overlay-minified:hidden">Account</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--message] size-5"></span>
          <span class="overlay-minified:hidden">Notifications</span>
        </a>
      </li>
      <li class="dropdown relative [--adaptive:none] [--strategy:static] overlay-minified:[--adaptive:adaptive] overlay-minified:[--strategy:fixed] overlay-minified:[--offset:15] overlay-minified:[--trigger:hover] overlay-minified:[--placement:right-start]" >
        <button id="dropdown-default" type="button" class="dropdown-toggle" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
        <span class="icon-[tabler--apps] size-5"></span>
          <span class="overlay-minified:hidden">Apps</span>
          <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4 overlay-minified:hidden" ></span>
        </button>
        <ul class="dropdown-menu mt-0 shadow-none overlay-minified:shadow-md overlay-minified:shadow-base-300/20 dropdown-open:opacity-100 hidden min-w-60 overlay-minified:before:absolute overlay-minified:before:-start-4 overlay-minified:before:top-0 overlay-minified:before:h-full overlay-minified:before:w-4 before:bg-transparent" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-default">
          <li>
              <a href="#">
                <span class="icon-[tabler--mail] size-5"></span>
                Email
              </a>
            </li>
            <li>
              <a href="#">
                <span class="icon-[tabler--calendar] size-5"></span>
                Calendar
              </a>
            </li>
        </ul>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--shopping-bag] size-5"></span>
          <span class="overlay-minified:hidden">Product</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--login] size-5"></span>
          <span class="overlay-minified:hidden">Sign In</span>
        </a>
      </li>
      <li>
        <a href="#">
          <span class="icon-[tabler--logout-2] size-5"></span>
          <span class="overlay-minified:hidden">Sign Out</span>
        </a>
      </li>
    </ul>
  </div>
</aside>
```
