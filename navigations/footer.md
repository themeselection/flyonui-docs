# Footer

The footer serves as a space where you can include various elements such as a logo, copyright notice, and links to other pages.

<!-- Class table -->

| Class | Type | Description |
| --- | --- | --- |
| footer | component | Base class for footer component. |
| footer-title | part | Base class for title of a footer column. |
| footer-center | modifier | Aligns footer content to center. |


<!-- Class Table -->

<!-------------------- Basic example -------------------->

## Basic example

<!-- Default -->

### Default

Use the component class `footer` for footer component.

```html
<div class="w-full">
  <footer class="footer items-center px-6 py-4">
    <aside class="grid-flow-col items-center">
      <p>&copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a></p>
    </aside>
    <nav class="text-base-content grid-flow-col gap-4 md:place-self-center md:justify-self-end">
      <a class="link link-hover" href="#">License</a>
      <a class="link link-hover" href="#">Help</a>
      <a class="link link-hover" href="#">Contact</a>
      <a class="link link-hover" href="#">Policy</a>
    </nav>
  </footer>
</div>
```

<!-------------------- Position -------------------->

## Position

<!-- Static footer -->

### Static footer

Use the component class `footer` for footer component. Below given example displays static footer with links.

```html
<div class="w-full">
  <!-- Demo content -->
  <div class="flex w-full flex-col gap-4">
    <div class="mb-4 flex items-center gap-4">
      <div class="skeleton h-16 w-16 shrink-0 rounded-full"></div>
      <div class="flex flex-col gap-4">
        <div class="skeleton h-4 w-52"></div>
        <div class="skeleton h-4 w-52"></div>
      </div>
    </div>
    <div class="skeleton mb-4 h-32 w-full"></div>
  </div>
  <!-- Static footer -->
  <footer class="footer bg-base-200/60 items-center rounded-t-box px-6 py-4 shadow-base-300/20 shadow-sm">
    <aside class="grid-flow-col items-center">
      <p>&copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a></p>
    </aside>
    <nav class="text-base-content grid-flow-col gap-4 md:place-self-center md:justify-self-end">
      <a class="link link-hover" href="#">License</a>
      <a class="link link-hover" href="#">Help</a>
      <a class="link link-hover" href="#">Contact</a>
      <a class="link link-hover" href="#">Policy</a>
    </nav>
  </footer>
</div>
```

<!-- Sticky footer -->

### Sticky footer

Please refer to the following example for a sticky footer that remains visible even when scrolling.

```html
<div class="relative h-60 w-full">
  <!-- Demo content -->
  <div class="overflow-y-auto relative h-full w-full overflow-y-scroll pe-2">
    <div class="flex w-full flex-col gap-4">
      <div class="mb-4 flex items-center gap-4">
        <div class="skeleton h-16 w-16 rounded-full"></div>
        <div class="flex flex-col gap-4">
          <div class="skeleton h-4 w-52"></div>
          <div class="skeleton h-4 w-52"></div>
        </div>
      </div>
      <div class="skeleton mb-4 h-16 w-full"></div>
      <div class="skeleton mb-4 h-32 w-full"></div>
    </div>
    <!-- Sticky Footer -->
    <footer class="footer bg-base-200 absolute -bottom-px sticky start-0 w-full px-6 py-4">
      <aside class="grid-flow-col items-center">
        <p>&copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a></p>
      </aside>
      <nav class="text-base-content grid-flow-col gap-4 md:place-self-center md:justify-self-end">
        <a class="link link-hover" href="#">License</a>
        <a class="link link-hover" href="#">Help</a>
        <a class="link link-hover" href="#">Contact</a>
        <a class="link link-hover" href="#">Policy</a>
      </nav>
    </footer>
  </div>
</div>
```

<!-------------------- Illustrations -------------------->

## Illustrations

<!-- With logo section -->

### With logo section

Please refer to the following example for a footer with logo section. Use component class `footer-title` for footer column headings.

```html
<footer class="footer bg-base-200/60 p-10">
  <aside class="gap-6">
    <div class="flex items-center gap-2 text-xl font-bold text-base-content">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z"
          fill="var(--color-primary)"
        /></svg>
      <span>FlyonUI</span>
    </div>
    <p class="text-base-content text-sm">Most developer friendly & highly <br />customisable Tailwind UI Kit. </p>
  </aside>
  <nav class="text-base-content">
    <h6 class="footer-title">Services</h6>
    <a href="#" class="link link-hover">Branding</a>
    <a href="#" class="link link-hover">Design</a>
    <a href="#" class="link link-hover">Marketing</a>
    <a href="#" class="link link-hover">Advertisement</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Company</h6>
    <a href="#" class="link link-hover">About us</a>
    <a href="#" class="link link-hover">Contact</a>
    <a href="#" class="link link-hover">Jobs</a>
    <a href="#" class="link link-hover">Press kit</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Legal</h6>
    <a href="#" class="link link-hover">Terms of use</a>
    <a href="#" class="link link-hover">Privacy policy</a>
    <a href="#" class="link link-hover">Cookie policy</a>
  </nav>
</footer>
```

<!-- With form -->

### With form

Please refer to the following example for a footer with form.

```html
<footer class="footer bg-base-200/60 p-10">
  <form class="gap-6">
    <div class="flex items-center gap-2 text-xl font-bold text-base-content">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z"
          fill="var(--color-primary)"
        /></svg>
      <span>FlyonUI</span>
    </div>
    <p class="text-base-content text-sm"> Most developer friendly & highly <br /> customisable Tailwind UI Kit. </p>
    <fieldset>
      <label class="label-text" for="subscribeLetter"> Subscribe to newsletter </label>
      <div class="flex w-full flex-wrap gap-1 sm:flex-nowrap">
        <input class="input input-sm" id="subscribeLetter" placeholder="johndoe@gmail.com" />
        <button class="btn btn-sm btn-primary" type="submit">Subscribe</button>
      </div>
    </fieldset>
  </form>
  <nav class="text-base-content">
    <h6 class="footer-title">Services</h6>
    <a href="#" class="link link-hover">Branding</a>
    <span>
      <a href="#" class="link link-hover">Design</a>
      <span class="badge badge-sm badge-primary ms-2">New</span>
    </span>
    <a href="#" class="link link-hover">Marketing</a>
    <a href="#" class="link link-hover">Advertisement</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Company</h6>
    <a href="#" class="link link-hover">About us</a>
    <a href="#" class="link link-hover">Contact</a>
    <a href="#" class="link link-hover">Jobs</a>
    <a href="#" class="link link-hover">Press kit</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Legal</h6>
    <a href="#" class="link link-hover">Terms of use</a>
    <a href="#" class="link link-hover">Privacy policy</a>
    <a href="#" class="link link-hover">Cookie policy</a>
  </nav>
</footer>
```

<!-- With Logo & Social Links -->

### With Logo & Social Links

Please refer to the following example for a footer with logo & social links.

```html
<footer class="footer bg-base-200/60 px-6 py-4">
  <div class="flex w-full flex-wrap items-center justify-between">
    <div class="flex items-center gap-2 text-xl font-bold text-base-content">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z"
          fill="var(--color-primary)"
        /></svg>
      <span>FlyonUI</span>
    </div>
    <aside class="grid-flow-col items-center">
      <p> &copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a> </p>
    </aside>
    <div class="flex h-5 gap-4">
      <a href="#" class="link" aria-label="Github Link">
        <span class="icon-[tabler--brand-github] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Facebook Link">
        <span class="icon-[tabler--brand-facebook] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="X Link">
        <span class="icon-[tabler--brand-x] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Google Link">
        <span class="icon-[tabler--brand-google] size-5"></span>
      </a>
    </div>
  </div>
</footer>
```

<!-- With copyright text -->

### With copyright text

Please refer to the following example for a footer with copyright text.

```html
<footer class="footer footer-center bg-base-200/60 px-6 py-4">
  <aside>
    <p>Copyright © 2024 - All right reserved.</p>
  </aside>
</footer>
```

<!-- With copyright text & social links -->

### With copyright text & social links

Please refer to the following example for a footer with copyright text & social links.

```html
<footer class="footer bg-base-200/60 px-6 py-4">
  <div class="flex w-full items-center justify-between">
  <aside class="grid-flow-col items-center">
    <p>&copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a></p>
  </aside>
    <div class="flex gap-4 h-5">
      <a href="#" class="link" aria-label="Github Link">
        <span class="icon-[tabler--brand-github] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Facebook Link">
        <span class="icon-[tabler--brand-facebook] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="X Link">
        <span class="icon-[tabler--brand-x] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Google Link">
        <span class="icon-[tabler--brand-google] size-5"></span>
      </a>
    </div>
  </div>
</footer>
```

<!-- With two rows -->

### With two rows

Please refer to the following example for a footer with two rows.

```html
<footer class="footer bg-base-200/60 grid-rows-2 p-10 text-base-content">
  <nav>
    <h6 class="footer-title">Services</h6>
    <a href="#" class="link link-hover">Branding</a>
    <a href="#" class="link link-hover">Design</a>
    <a href="#" class="link link-hover">Marketing</a>
    <a href="#" class="link link-hover">Advertisement</a>
  </nav>
  <nav>
    <h6 class="footer-title">Company</h6>
    <a href="#" class="link link-hover">About us</a>
    <a href="#" class="link link-hover">Contact</a>
    <a href="#" class="link link-hover">Jobs</a>
    <a href="#" class="link link-hover">Press kit</a>
  </nav>
  <nav>
    <h6 class="footer-title">Legal</h6>
    <a href="#" class="link link-hover">Terms of use</a>
    <a href="#" class="link link-hover">Privacy policy</a>
    <a href="#" class="link link-hover">Cookie policy</a>
  </nav>
  <nav>
    <h6 class="footer-title">Social</h6>
    <a href="#" class="link link-hover">Twitter</a>
    <a href="#" class="link link-hover">Instagram</a>
    <a href="#" class="link link-hover">Facebook</a>
    <a href="#" class="link link-hover">Github</a>
  </nav>
  <nav>
    <h6 class="footer-title">Explore</h6>
    <a href="#" class="link link-hover">Features</a>
    <a href="#" class="link link-hover">Enterprise</a>
    <a href="#" class="link link-hover">Security</a>
    <a href="#" class="link link-hover">Pricing</a>
  </nav>
  <nav>
    <h6 class="footer-title">Apps</h6>
    <a href="#" class="link link-hover">Mac</a>
    <a href="#" class="link link-hover">Windows</a>
    <a href="#" class="link link-hover">iPhone</a>
    <a href="#" class="link link-hover">Android</a>
  </nav>
</footer>
```

<!-- Centered footer with logo & social icons -->

### Centered footer with logo & social icons

Please refer to the example below for a centered footer with a logo and social icons. Utilize the modifier class `footer-center` to align the footer content in the center.

```html
<footer class="footer bg-base-200/60 flex flex-col items-center gap-4 p-6">
  <div class="flex items-center gap-2 text-xl font-bold text-base-content">
    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z"
          fill="var(--color-primary)"
        /></svg>
    <span>FlyonUI</span>
  </div>
  <aside>
    <p>©2024<span class="font-medium">FlyonUI</span></p>
  </aside>
  <nav class="grid-flow-col gap-4">
    <a class="link link-hover text-base-content" href="#">License</a>
    <a class="link link-hover text-base-content" href="#">Help</a>
    <a class="link link-hover text-base-content" href="#">Contact</a>
    <a class="link link-hover text-base-content" href="#">Policy</a>
  </nav>
  <div class="flex h-5 gap-4">
    <a href="#" class="link text-base-content" aria-label="Github Link">
      <span class="icon-[tabler--brand-github-filled] size-5"></span>
    </a>
    <a href="#" class="link text-base-content" aria-label="Facebook Link">
      <span class="icon-[tabler--brand-facebook-filled] size-5"></span>
    </a>
    <a href="#" class="link text-base-content" aria-label="X Link">
      <span class="icon-[tabler--brand-x-filled] size-5"></span>
    </a>
    <a href="#" class="link text-base-content" aria-label="Google Link">
      <span class="icon-[tabler--brand-google-filled] size-5"></span>
    </a>
  </div>
</footer>
```

<!-- Centered footer with social icons -->

### Centered footer with social icons

Please refer to the example below for a centered footer with social icons.

```html
<footer class="footer footer-center bg-base-200/60 rounded-sm p-6">
  <nav class="grid grid-flow-col gap-4 text-base-content">
    <a href="#" class="link link-hover">About</a>
    <a href="#" class="link link-hover">Contact</a>
    <a href="#" class="link link-hover">Jobs</a>
    <a href="#" class="link link-hover">Policy</a>
  </nav>
  <nav>
    <div class="flex gap-4">
      <a href="#" class="link link-animated" aria-label="Facebook Link">
        <span class="icon-[tabler--brand-facebook] size-6"></span>
      </a>
      <a href="#" class="link link-animated" aria-label="X Link">
        <span class="icon-[tabler--brand-x] size-6"></span>
      </a>
      <a href="#" class="link link-animated" aria-label="Linkedin Link">
        <span class="icon-[tabler--brand-linkedin] size-6"></span>
      </a>
    </div>
  </nav>
  <aside>
    <p>Copyright © 2024 - All right reserved by FlyonUI</p>
  </aside>
</footer>
```

<!-- Dual footer (with partition) -->

### Dual footer (with partition)

Please refer to the example below for a footer dual footer with partition.

```html
<div class="w-full">
<footer class="footer bg-base-200/60 p-10">
  <form class="gap-6">
    <div class="flex items-center gap-2 text-xl font-bold text-base-content">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.6745 16.9224L12.6233 10.378C12.2167 9.85117 11.4185 9.8611 11.0251 10.3979L6.45728 16.631C6.26893 16.888 5.96935 17.0398 5.65069 17.0398H3.79114C2.9635 17.0398 2.49412 16.0919 2.99583 15.4336L11.0224 4.90319C11.4206 4.38084 12.2056 4.37762 12.608 4.89668L20.9829 15.6987C21.4923 16.3558 21.024 17.3114 20.1926 17.3114H18.4661C18.1562 17.3114 17.8638 17.1677 17.6745 16.9224ZM12.5866 15.5924L14.8956 18.3593C15.439 19.0105 14.976 20 14.1278 20H9.74075C8.9164 20 8.4461 19.0586 8.94116 18.3994L11.0192 15.6325C11.4065 15.1169 12.1734 15.0972 12.5866 15.5924Z"
          fill="var(--color-primary)"
        /></svg>
      <span>FlyonUI</span>
    </div>
    <p class="text-base-content text-sm">Most developer friendly & highly<br />customisable Tailwind UI Kit.</p>
    <fieldset>
      <label class="label-text" for="subscribeNewsletter"> Subscribe to newsletter </label>
      <div class="flex flex-wrap sm:flex-nowrap w-full gap-1">
        <input class="input input-sm" id="subscribeNewsletter" placeholder="johndoe@gmail.com" />
        <button class="btn btn-sm btn-primary">Subscribe</button>
      </div>
    </fieldset>
  </form>
  <nav class="text-base-content">
    <h6 class="footer-title">Services</h6>
    <a href="#" class="link link-hover">Branding</a>
    <span><a href="#" class="link link-hover">Design</a><span class="badge ms-2 badge-sm badge-primary">New</span></span>
    <a href="#" class="link link-hover">Marketing</a>
    <a href="#" class="link link-hover">Advertisement</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Company</h6>
    <a href="#" class="link link-hover">About us</a>
    <a href="#" class="link link-hover">Contact</a>
    <a href="#" class="link link-hover">Jobs</a>
    <a href="#" class="link link-hover">Press kit</a>
  </nav>
  <nav class="text-base-content">
    <h6 class="footer-title">Legal</h6>
    <a href="#" class="link link-hover">Terms of use</a>
    <a href="#" class="link link-hover">Privacy policy</a>
    <a href="#" class="link link-hover">Cookie policy</a>
  </nav>
</footer>
<footer class="footer bg-base-200/60 border-base-content/25 border-t px-6 py-4">
  <div class="flex w-full items-center justify-between">
    <aside class="grid-flow-col items-center">
      <p>&copy;2024 <a class="link link-hover font-medium" href="#">FlyonUI</a></p>
    </aside>
    <div class="flex h-5 gap-4">
      <a href="#" class="link" aria-label="Github Link">
        <span class="icon-[tabler--brand-github] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Facebook Link">
        <span class="icon-[tabler--brand-facebook] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="X Link">
        <span class="icon-[tabler--brand-x] size-5"></span>
      </a>
      <a href="#" class="link" aria-label="Google Link">
        <span class="icon-[tabler--brand-google] size-5"></span>
      </a>
    </div>
  </div>
</footer>
</div>
```

<!-- With dropdown -->

### With dropdown

  Please refer to the example below for a footer with dropdown.

```html
<footer class="footer grid-flow-col bg-base-200/60 items-center p-4">
  <aside class="grid-flow-col items-center">
    <a class="link link-hover font-medium" href="#">FlyonUI &copy;</a>
  </aside>
  <nav class="grid-flow-col gap-4 place-items-center place-self-center justify-self-end">
    <div>
      <div class="dropdown relative inline-flex">
        <button id="dropdown-dividers" type="button" class="dropdown-toggle btn btn-secondary btn-outline btn-sm" aria-haspopup="menu" aria-expanded="false" aria-label="Dropdown">
          Currency
          <span class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"></span>
        </button>
        <ul class="dropdown-menu dropdown-open:opacity-100 hidden min-w-20" role="menu" aria-orientation="vertical" aria-labelledby="dropdown-dividers">
          <li><a class="dropdown-item" href="#">$ USD</a></li>
          <li><a class="dropdown-item" href="#">&euro; Euro</a></li>
          <li><a class="dropdown-item" href="#">£ Pound</a></li>
          <li><a class="dropdown-item" href="#">₹ Rupee</a></li>
          <li><hr class="border-base-content/25 -mx-2 my-3" /></li>
          <li><a class="dropdown-item" href="#">₿ Bitcoin</a></li>
        </ul>
      </div>
    </div>
    <a class="btn btn-outline btn-error btn-sm max-sm:btn-square" href="#">
      <span class="max-sm:hidden">Logout</span>
      <span class="icon-[tabler--logout]"></span>
    </a>
  </nav>
</footer>
```
