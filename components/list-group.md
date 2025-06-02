# List Group

List groups provide a flexible framework for displaying a sequence of content. They can be customized and expanded to fit virtually any type of content.

<!-------------------- Basic -------------------->

## Basic example

<!-- Default -->

### Default

The most basic list group is an unordered list with list items.

```html
<ul
  class="border-base-content/25 divide-base-content/25 w-96 divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md">
  <li>Recent Posts</li>
  <li>Upcoming Events</li>
  <li>Notifications</li>
</ul>
```

<!-------------------- State -------------------->

## State

<!-- Link -->

### Link

Use the `<a>` tag to create interactive list group items that exhibit hover, active, and disabled states. The `link` component class aids in styling these links and buttons for consistency.

```html
<div
  class="border-base-content/25 divide-base-content/25 flex w-96 flex-col divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md">
  <a href="#" class="link link-primary flex items-center no-underline">
    <span class="icon-[tabler--activity] me-3 size-5"></span>
      Active
  </a>
  <a href="#" class="link hover:link-primary flex items-center no-underline">
    <span class="icon-[tabler--link] me-3 size-5"></span>
      Link
  </a>
  <a href="#" class="link flex items-center no-underline" disabled>
    <span class="icon-[tabler--ban] me-3 size-5"></span>
      Disabled
  </a>
</div>
```

<!-- Button -->

### Button

Use the `button` element to develop interactive list group items that include hover, active, and disabled states.

```html
<div
  class="border-base-content/25 divide-base-content/25 flex w-96 flex-col divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md">
  <button class="link link-primary flex items-center no-underline">
    <span class="icon-[tabler--activity] me-3 size-5"></span>
      Active
  </button>
  <button class="link hover:link-primary flex items-center no-underline">
    <span class="icon-[tabler--link] me-3 size-5"></span>
      Link
  </button>
  <button class="link flex items-center no-underline" disabled>
    <span class="icon-[tabler--ban] me-3 size-5"></span>
      Disabled
  </button>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- Icons -->

### Icons

The standard list group featuring icons.

```html
<ul class="border-base-content/25 divide-base-content/25 w-96 divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md">
  <li class="flex items-center ">
    <span class="icon-[tabler--user] text-base-content me-3 size-5"></span>
    Recent Posts
  </li>
  <li class="flex items-center">
    <span class="icon-[tabler--calendar-event] text-base-content me-3 size-5"></span>Upcoming Events
  </li>
  <li class="flex items-center">
    <span class="icon-[tabler--message] text-base-content me-3 size-5"></span>Notifications
  </li>
</ul>
```

<!-- Badge -->

### Badge

Incorporate `badges` into any list group item to display unread Notifications, activity levels, and additional information.

```html
<ul class="border-base-content/25 divide-base-content/25 w-96 divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md">
  <li class="flex items-center justify-between">
    Recent Posts <span class="badge badge-primary rounded-full">New</span>
  </li>
  <li class="flex items-center justify-between">
    Upcoming Events <span class="badge badge-primary rounded-full">2</span>
  </li>
  <li class="flex items-center justify-between">
    Notifications <span class="badge badge-primary rounded-full">+99</span>
  </li>
</ul>
```

<!-- Horizontal -->

### Horizontal

The horizontal list will change to vertical order at small resolutions. Reduce browser size to see it in action.

```html
<div class="w-full">
  <ul class="border-base-content/25 divide-base-content/25 rounded-md flex w-full flex-col border *:w-full *:cursor-pointer max-sm:divide-y sm:flex-row sm:divide-x *:p-3" >
    <li class="w-full">Recent Posts</li>
    <li class="w-full">Upcoming Events</li>
    <li class="w-full">Notifications</li>
  </ul>
</div>
```

<!-- Flush -->

### Flush

Eliminate certain borders and soften the corners to allow list group items to fit seamlessly edge-to-edge within a parent container, such as cards.

```html
<ul class="divide-base-content/25 w-96 divide-y *:p-3">
  <li>Recent Posts</li>
  <li>Upcoming Events</li>
  <li>Notifications</li>
</ul>
```

<!-- No gutters -->

### No gutters

No paddings in left and right.

```html
<ul class="divide-base-content/25 w-96 divide-y *:py-3">
  <li>Recent Posts</li>
  <li>Upcoming Events</li>
  <li>Notifications</li>
</ul>
```

<!-- Striped -->

### Striped

Applying alternate shading to list items.

```html
<ul class="border-base-content/25 divide-base-content/25 w-96 divide-y rounded-md border *:p-3 *:first:rounded-t-md *:last:rounded-b-md *:odd:bg-base-200">
  <li>Recent Posts</li>
  <li>Upcoming Events</li>
  <li>Downloads</li>
  <li>Team Account</li>
  <li>Notifications</li>
</ul>
```

<!-- Checkbox -->

### Checkbox

List group with checkbox.

```html
<h6 class="text-base text-base-content mb-1">Select your skills:</h6>
<ul class="border-base-content/25 divide-base-content/25 divide-y max-w-sm rounded-md border *:first:rounded-t-md *:last:rounded-b-md *:cursor-pointer">
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> Web Development </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" checked />
      <span class="label-text text-base"> Data Analysis </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="checkbox checkbox-primary" />
      <span class="label-text text-base"> Graphic Design </span>
    </label>
  </li>
</ul>
```

<!-- Radio -->

### Radio

List group with radio.

```html
<h6 class="text-base text-base-content mb-1">Select your expertise:</h6>
<ul class="border-base-content/25 divide-base-content/25 divide-y max-w-sm rounded-md border *:first:rounded-t-md *:last:rounded-b-md *:cursor-pointer">
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="radio" name="radio-13" class="radio radio-primary" />
      <span class="label-text text-base"> Project Management </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="radio" name="radio-13" class="radio radio-primary" checked />
      <span class="label-text text-base"> Marketing Strategy </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="radio" name="radio-13" class="radio radio-primary" />
      <span class="label-text text-base"> Financial Analysis </span>
    </label>
  </li>
</ul>
```

<!-- Switch -->

### Switch

List group with switch.

```html
<h6 class="text-base text-base-content mb-1">Switch your preferred certifications:</h6>
<ul class="border-base-content/25 max-w-sm divide-base-content/25 divide-y rounded-md border *:first:rounded-t-md *:last:rounded-b-md *:cursor-pointer">
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> Project Management </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" checked />
      <span class="label-text text-base"> Certified ScrumMaster </span>
    </label>
  </li>
  <li>
    <label class="flex items-center gap-3 p-3">
      <input type="checkbox" class="switch switch-primary" />
      <span class="label-text text-base"> Google Analytics </span>
    </label>
  </li>
</ul>
```

<!-- Invoice list group -->

### Invoice list group

An example of a basic list group with an emphasized footer.

```html
<ul class="border-base-content/25 divide-base-content/25 divide-y rounded-md border *:first:rounded-t-md *:last:rounded-b-md *:p-3 w-96">
    <li class="flex justify-between items-center">Payment to Front <span class="text-base-content">&#8377; 264</span></li>
    <li class="flex justify-between items-center">Discount <span class="text-base-content">&#8377; 50</span></li>
    <li class="flex justify-between items-center bg-base-200">Amount paid <span class="text-base-content">&#8377; 214</span></li>
</ul>
```

<!-- User list -->

### User list

Presenting user profiles in a structured list group format.

```html
<div class="w-full md:w-1/2">
  <ul class="border-base-content/25 divide-base-content/25 *:last:rounded-b-md divide-y rounded-md border *:p-3 *:first:rounded-t-md" >
    <li class="flex items-start sm:items-center">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Image" class="w-13 me-3 rounded-full" />
      <div class="flex grow flex-col items-start justify-between sm:flex-row">
        <div>
          <h6 class="text-base text-base-content">Danish sesame snaps halvah</h6>
          <small class="text-base-content/50 text-sm">13 minutes</small>
          <div class="w-full">
            <span class="bg-success inline-block size-2 rounded-full"></span>
            <small>Online</small>
          </div>
        </div>
        <div class="action max-sm:mt-1">
          <button class="btn btn-primary btn-sm">Add</button>
        </div>
      </div>
    </li>
    <li class="flex items-start sm:items-center">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Image" class="w-13 me-3 rounded-full" />
      <div class="flex grow flex-col items-start justify-between sm:flex-row">
        <div>
          <h6 class="text-base text-base-content">Cake halvah biscuit cheesecake</h6>
          <small class="text-base-content/50 text-sm">11 minutes</small>
          <div class="w-full">
            <span class="bg-warning inline-block size-2 rounded-full"></span>
            <small>Away</small>
          </div>
        </div>
        <div class="action max-sm:mt-1">
          <button class="btn btn-primary btn-sm">Add</button>
        </div>
      </div>
    </li>
    <li class="flex items-start sm:items-center">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-6.png" alt="User Image" class="w-13 me-3 rounded-full" />
      <div class="flex grow flex-col items-start justify-between sm:flex-row">
        <div>
          <h6 class="text-base text-base-content">Tart cheesecake jujubes caramels</h6>
          <small class="text-base-content/50 text-sm">7 minutes</small>
          <div class="w-full">
            <span class="bg-secondary inline-block size-2 rounded-full"></span>
            <small>Offline</small>
          </div>
        </div>
        <div class="action max-sm:mt-1">
          <button class="btn btn-primary btn-sm">Add</button>
        </div>
      </div>
    </li>
    <li class="flex items-start sm:items-center">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-7.png" alt="User Image" class="w-13 me-3 rounded-full" />
      <div class="flex grow flex-col items-start justify-between sm:flex-row">
        <div>
          <h6 class="text-base text-base-content">Icing sweet gummies</h6>
          <small class="text-base-content/50 text-sm">15 minutes</small>
          <div class="w-full">
            <span class="bg-error inline-block size-2 rounded-full"></span>
            <small>In meeting</small>
          </div>
        </div>
        <div class="action max-sm:mt-1">
          <button class="btn btn-primary btn-sm">Add</button>
        </div>
      </div>
    </li>
  </ul>
</div>
```

<!-- Progress -->

### Progress

A list group displaying progress indicators.

```html
<ul class="border-base-content/25 divide-base-content/25 *:last:rounded-b-md divide-y rounded-md border *:p-3 *:first:rounded-t-md w-full" >
    <li class="flex items-start">
      <div class="avatar avatar-placeholder me-3">
        <div class="bg-info text-info-content w-10 rounded-lg">
          <span class="icon-[tabler--brand-tailwind] size-6"></span>
        </div>
      </div>
      <div class="grow">
        <h6 class="text-base text-base-content mb-2">Bootstrap is an open source toolkit</h6>
        <div class="progress h-2 w-full" role="progressbar" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100">
          <div class="progress-bar progress-info w-1/2"></div>
        </div>
      </div>
    </li>
    <li class="flex items-start">
      <div class="avatar avatar-placeholder me-3">
        <div class="bg-success text-success-content w-10 rounded-lg">
          <span class="icon-[tabler--brand-vue] size-6"></span>
        </div>
      </div>
      <div class="grow">
        <h6 class="text-base text-base-content mb-2">Vue.js is the Progressive JavaScript Framework</h6>
        <div class="progress h-2 w-full" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">
          <div class="progress-bar progress-success w-1/2"></div>
        </div>
      </div>
    </li>
    <li class="flex items-start">
      <div class="avatar avatar-placeholder me-3">
        <div class="bg-error text-error-content w-10 rounded-lg">
          <span class="icon-[tabler--brand-angular] size-6"></span>
        </div>
      </div>
      <div class="grow">
        <h6 class="text-base text-base-content mb-2 text-ellipsis">Angular implements Functional Programming concepts</h6>
        <div class="progress h-2 w-full" role="progressbar" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100">
          <div class="progress-bar progress-error w-1/2"></div>
        </div>
      </div>
    </li>
    <li class="flex items-start">
      <div class="avatar avatar-placeholder me-3">
        <div class="bg-primary text-primary-content w-10 rounded-lg">
          <span class="icon-[tabler--brand-react] size-6"></span>
        </div>
      </div>
      <div class="grow">
        <h6 class="text-base text-base-content mb-2">React version update</h6>
        <div class="progress h-2 w-full" role="progressbar" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">
          <div class="progress-bar progress-primary w-1/2"></div>
        </div>
      </div>
    </li>
  </ul>
```

<!-------------------- Cards -------------------->

## Cards

<!-- List Item with Icon -->

### List Item with Icon

Present a list item with an icon in a structured card layout.

```html
<div class="card w-80">
  <div class="text-base-content/50 text-sm font-medium px-4 py-2">USER PROFILE</div>
  <li class="flex items-center px-4 py-2.5">
    <span class="icon-[tabler--user] me-2 size-5"></span>
    Profile
  </li>
  <li class="flex items-center px-4 py-2.5">
    <span class="icon-[tabler--settings] me-2 size-5"></span>
    Settings
  </li>
  <li class="flex items-center px-4 py-2.5">
    <span class="icon-[tabler--file-dollar] me-2 size-5"></span>
    Billing Plans
  </li>
  <li class="flex items-center px-4 py-2.5">
    <span class="icon-[tabler--currency-dollar] me-2 size-5"></span>
    Pricing
  </li>
  <li class="flex items-center px-4 py-2.5">
    <span class="icon-[tabler--question-mark] me-2 size-5"></span>
    FAQ
  </li>
</div>
```

<!-- List Item with Switch -->

### List Item with Switch

Organize a list item with a switch in a well-structured card.

```html
<div class="card w-80">
  <div class="text-base-content/50 px-4 py-2 text-sm font-medium">APPS NOTIFICATION</div>
  <ul class="space-y-0.5">
    <li class="flex items-center justify-between px-4 py-2.5">
      <div class="flex items-center gap-2">
        <img src="https://cdn.flyonui.com/fy-assets/components/social-icon/google.png" alt="google" class="size-5" />
        <span>Google</span>
      </div>
      <input type="checkbox" class="switch switch-primary" />
    </li>
    <li class="flex items-center justify-between px-4 py-2.5">
      <div class="flex items-center gap-2">
        <img src="https://cdn.flyonui.com/fy-assets/components/social-icon/twitter.png" alt="twitter" class="size-5" />
        <span>Twitter</span>
      </div>
      <input type="checkbox" class="switch switch-primary" />
    </li>
    <li class="flex items-center justify-between px-4 py-2.5">
      <div class="flex items-center gap-2">
        <img src="https://cdn.flyonui.com/fy-assets/components/social-icon/linkedin.png" alt="linkedin" class="size-5" />
        <span>Linkedin</span>
      </div>
      <input type="checkbox" class="switch switch-primary" />
    </li>
    <li class="flex items-center justify-between px-4 py-2.5">
      <div class="flex items-center gap-2">
        <img src="https://cdn.flyonui.com/fy-assets/components/social-icon/dribbble.png" alt="dribble" class="size-5" />
        <span>Dribbble</span>
      </div>
      <input type="checkbox" class="switch switch-primary" />
    </li>
    <li class="flex items-center justify-between px-4 py-2.5">
      <div class="flex items-center gap-2">
        <img src="https://cdn.flyonui.com/fy-assets/components/social-icon/behance.png" alt="behance" class="size-5" />
        <span>Behance</span>
      </div>
      <input type="checkbox" class="switch switch-primary" />
    </li>
  </ul>
</div>
```

<!-- List Item With Action -->

### List Item With Action

Include a list item with an action option in a structured card format.

```html
<div class="card w-96">
  <div class="text-base-content/50 px-4 py-2 text-sm font-medium">CONTACT LIST</div>
  <li class="flex items-center gap-2 px-4 py-2.5">
    <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Image" class="size-10 rounded-full" />
    <div class="flex grow items-center justify-between gap-y-1">
      <div>
        <h6 class="text-base">Angel Dorwart</h6>
        <small class="text-base-content/80 text-xs">sbaker@hotmail.com</small>
      </div>
      <div class="action max-sm:mt-1">
        <button class="btn btn-soft btn-sm max-sm:btn-square"> <span class="icon-[tabler--send]"></span> <span class="max-sm:hidden">Send</span> </button>
      </div>
    </div>
  </li>
  <li class="flex items-center gap-2 px-4 py-2.5">
    <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Image" class="size-10 rounded-full" />
    <div class="flex grow items-center justify-between gap-y-1">
      <div>
        <h6 class="text-base">Skylar Rosser</h6>
        <small class="text-base-content/80 text-xs">gbaker@yahoo.com</small>
      </div>
      <div class="action max-sm:mt-1">
        <button class="btn btn-soft btn-sm max-sm:btn-square"> <span class="icon-[tabler--send]"></span> <span class="max-sm:hidden">Send</span> </button>
      </div>
    </div>
  </li>
  <li class="flex items-center gap-2 px-4 py-2.5">
    <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Image" class="size-10 rounded-full" />
    <div class="flex grow items-center justify-between gap-y-1">
      <div>
        <h6 class="text-base">Dulce Botosh</h6>
        <small class="text-base-content/80 text-xs">tlee@gmail.com</small>
      </div>
      <div class="action max-sm:mt-1">
        <button class="btn btn-soft btn-sm max-sm:btn-square"> <span class="icon-[tabler--send]"></span> <span class="max-sm:hidden">Send</span> </button>
      </div>
    </div>
  </li>
  <li class="flex items-center gap-2 px-4 py-2.5">
    <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Image" class="size-10 rounded-full" />
    <div class="flex grow items-center justify-between gap-y-1">
      <div>
        <h6 class="text-base">Ahmad Stanton</h6>
        <small class="text-base-content/80 text-xs">kdavis@hotmail.com</small>
      </div>
      <div class="action max-sm:mt-1">
        <button class="btn btn-soft btn-sm max-sm:btn-square"> <span class="icon-[tabler--send]"></span> <span class="max-sm:hidden">Send</span> </button>
      </div>
    </div>
  </li>
  <li class="flex items-center gap-2 px-4 py-2.5">
    <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-5.png" alt="User Image" class="size-10 rounded-full" />
    <div class="flex grow items-center justify-between gap-y-1">
      <div>
        <h6 class="text-base-content text-base">Randy Gouse</h6>
        <small class="text-base-content/80 text-xs">ijackson@yahoo.com</small>
      </div>
      <div class="action max-sm:mt-1">
        <button class="btn btn-soft btn-sm max-sm:btn-square"> <span class="icon-[tabler--send]"></span> <span class="max-sm:hidden">Send</span> </button>
      </div>
    </div>
  </li>
  <div class="card-footer">
    <button class="btn btn-primary btn-block btn-gradient">Add Contact</button>
  </div>
</div>
```

<!-- List Item With Avatar -->

### List Item With Avatar

Presenting List Item With Avatar in a structured card layout.

```html
<div class="card w-96">
  <div class="text-base-content/50 px-4 py-2 text-sm font-medium">CHAT LIST</div>
  <ul class="space-y-0.5">
    <li class="flex items-center gap-2 px-4 py-2.5">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Image" class="size-10 rounded-full" />
      <div class="flex grow items-center justify-between gap-y-1">
        <div>
          <h6 class="text-base">Phillip George</h6>
          <small class="text-base-content/80 text-xs">Hii samira, thanks for...</small>
        </div>
        <div class="flex flex-col items-end gap-x-2 gap-y-0.5">
          <span class="text-base-content/50 text-xs">9.00AM</span>
          <span class="badge badge-success badge-xs rounded-full">1</span>
        </div>
      </div>
    </li>
    <li class="flex items-center gap-2 px-4 py-2.5">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-2.png" alt="User Image" class="size-10 rounded-full" />
      <div class="flex grow items-center justify-between gap-y-1">
        <div>
          <h6 class="text-base">Jaylon Donin</h6>
          <small class="text-base-content/80 text-xs">I’ll send the texts...</small>
        </div>
        <div class="flex flex-col items-end gap-x-2 gap-y-0.5">
          <span class="text-base-content/50 text-xs">10.00PM</span>
          <span class="badge badge-success badge-xs rounded-full">3</span>
        </div>
      </div>
    </li>
    <li class="flex items-center gap-2 px-4 py-2.5">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-3.png" alt="User Image" class="size-10 rounded-full" />
      <div class="flex grow items-center justify-between gap-y-1">
        <div>
          <h6 class="text-base">Tiana Curtis</h6>
          <small class="text-base-content/80 text-xs">That’s Great!</small>
        </div>
        <span class="text-base-content/50 text-xs">8.30AM</span>
      </div>
    </li>
    <li class="flex items-center gap-2 px-4 py-2.5">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-4.png" alt="User Image" class="size-10 rounded-full" />
      <div class="flex grow items-center justify-between gap-y-1">
        <div>
          <h6 class="text-base">Zaire Vetrovs</h6>
          <small class="text-base-content/80 text-xs">https://www.youtub...</small>
        </div>
        <div class="flex flex-col items-end gap-x-2 gap-y-0.5">
          <span class="text-base-content/50 text-xs">5.50AM</span>
          <span class="badge badge-success badge-xs rounded-full">2</span>
        </div>
      </div>
    </li>
    <li class="flex items-center gap-2 px-4 py-2.5">
      <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-5.png" alt="User Image" class="size-10 rounded-full" />
      <div class="flex grow items-center justify-between gap-y-1">
        <div>
          <h6 class="text-base">Kianna Philips</h6>
          <small class="text-base-content/80 text-xs">It was awesome.</small>
        </div>
        <span class="text-base-content/50 text-xs">6.45PM</span>
      </div>
    </li>
  </ul>
</div>
```

<!-- List Item Advanced -->

### List Item Advanced

Displaying an advanced list item in a structured card format.

```html
<div class="card w-full">
  <div class="text-base-content/50 px-2 py-2 text-sm font-medium sm:px-4">TODAY’S MEETINGS</div>
  <ul class="space-y-0.5">
    <li class="flex items-center px-2 py-2.5 max-sm:gap-4 sm:gap-8 sm:px-4">
      <span class="min-w-14 text-xl font-medium">08:30</span>
      <div class="w-full">
        <h6 class="text-base font-medium">Daily Project Review</h6>
        <small class="text-base-content/80 text-xs max-sm:hidden">Team organization</small>
      </div>
      <div class="avatar max-sm:hidden">
        <div class="size-9.5 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-1.png" alt="User Image" />
        </div>
      </div>
      <div class="flex items-center gap-1">
        <label class="label-text text-base max-sm:hidden" for="privacy1"> Privacy </label>
        <input type="checkbox" class="switch switch-primary max-[480px]:hidden" id="privacy1" />
      </div>
    </li>
    <li class="flex items-center px-2 py-2.5 max-sm:gap-4 sm:gap-8 sm:px-4">
      <span class="min-w-14 text-xl font-medium">09:00</span>
      <div class="w-full">
        <h6 class="text-base font-medium">Sprint Surge</h6>
        <small class="text-base-content/80 text-xs max-sm:hidden">Daily Boost for Agile Progress</small>
      </div>
      <div class="avatar-group -space-x-4 max-sm:hidden">
        <div class="avatar">
          <div class="w-9.5">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-10.png" alt="User Image" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-9.5">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-6.png" alt="User Image" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-9.5">
            <span>+9</span>
          </div>
        </div>
      </div>
      <div class="flex items-center gap-1">
        <label class="label-text text-base max-sm:hidden" for="privacy2"> Privacy </label>
        <input type="checkbox" class="switch switch-primary max-[480px]:hidden" id="privacy2" checked />
      </div>
    </li>
    <li class="flex items-center px-2 py-2.5 max-sm:gap-4 sm:gap-8 sm:px-4">
      <span class="min-w-14 text-xl font-medium">11:45</span>
      <div class="w-full">
        <h6 class="text-base font-medium">Project Status Update</h6>
        <small class="text-base-content/80 text-xs max-sm:hidden">Progress Overview Update</small>
      </div>
      <div class="avatar max-sm:hidden">
        <div class="size-9.5 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-8.png" alt="User Image" />
        </div>
      </div>
      <div class="flex items-center gap-1">
        <label class="label-text text-base max-sm:hidden" for="privacy3"> Privacy </label>
        <input type="checkbox" class="switch switch-primary max-[480px]:hidden" id="privacy3" />
      </div>
    </li>
    <li class="flex items-center px-2 py-2.5 max-sm:gap-4 sm:gap-8 sm:px-4">
      <span class="min-w-14 text-xl font-medium">06:30</span>
      <div class="w-full">
        <h6 class="text-base font-medium">Team Performance</h6>
        <small class="text-base-content/80 text-xs max-sm:hidden">Team Metrics Evaluation</small>
      </div>
      <div class="avatar-group -space-x-4 max-sm:hidden">
        <div class="avatar">
          <div class="w-9.5">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-10.png" alt="User Image" />
          </div>
        </div>
        <div class="avatar">
          <div class="w-9.5">
            <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-6.png" alt="User Image" />
          </div>
        </div>
        <div class="avatar avatar-placeholder">
          <div class="bg-neutral text-neutral-content w-9.5">
            <span>+9</span>
          </div>
        </div>
      </div>
      <div class="flex items-center gap-1">
        <label class="label-text text-base max-sm:hidden" for="privacy4"> Privacy </label>
        <input type="checkbox" class="switch switch-primary max-[480px]:hidden" id="privacy4" checked />
      </div>
    </li>
    <li class="flex items-center px-2 py-2.5 max-sm:gap-4 sm:gap-8 sm:px-4">
      <span class="min-w-14 text-xl font-medium">10:50</span>
      <div class="w-full">
        <h6 class="text-base font-medium">Stakeholder Feedback</h6>
        <small class="text-base-content/80 text-xs max-sm:hidden">Feedback from Stakeholders</small>
      </div>
      <div class="avatar max-sm:hidden">
        <div class="size-9.5 rounded-full">
          <img src="https://cdn.flyonui.com/fy-assets/avatar/avatar-7.png" alt="User Image" />
        </div>
      </div>
      <div class="flex items-center gap-1">
        <label class="label-text text-base max-sm:hidden" for="privacy5"> Privacy </label>
        <input type="checkbox" class="switch switch-primary max-[480px]:hidden" id="privacy5" />
      </div>
    </li>
  </ul>
</div>
```
