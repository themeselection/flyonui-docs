# Set up FlyonUI with Tailwind CSS Qwik

Combine FlyonUI with Qwik and Tailwind CSS to build a sleek, responsive interface, optimizing your development workflow for greater efficiency.

> **Info:** <h2 class="text-lg font-medium">Installation</h2>
> Please note that the plugin has been tested with the latest version of the framework (v1.12.1). The framework was installed using the standard <code>`npm create qwik@latest`</code> command. If you are using your own project structure, be mindful of file paths!

<div>
  <div class="flex gap-2">
    <div><img src="https://cdn.flyonui.com/fy-assets/icons/qwik-icon.png" alt="Qwik logo" class="h-auto w-14 mt-2" /></div>
    <div>
      <h2 class="text-base-content mb-3 text-lg font-semibold mt-2">
        Quick
        <span class="text-sky-500">Qwik</span>
        setup
      </h2>
      <p class="text-base-conte/80 text-base">
        <a href="https://qwik.dev/" class="link link-animated link-primary" target="_blank">Qwik</a> is an instant-loading framework with minimal overhead. If you haven't set up Tailwind CSS yet, check out 
        <a class="link link-animated" target="_blank" href="https://tailwindcss.com/docs/installation/framework-guides/qwik">
          Qwik Tailwind CSS
        </a>
        installation guides.
      </p>
      <div class="tooltip">
        <a href="https://github.com/themeselection/flyonui-qwik-integration" target="_blank" type="button" class="tooltip-toggle btn-sm btn btn-outline" aria-label="Tooltip">
          <span class="icon-[tabler--brand-github] size-4"></span>
          FlyonUI + Qwik
        </a>
        <span class="tooltip-content tooltip-shown:opacity-100 tooltip-shown:visible" role="tooltip">
          <span class="tooltip-body">Check out the starterkit</span>
        </span>
      </div>
       <p class="!mb-2 !mt-4">This repository consists of two branches:</p>
      <ul class="!my-2">
        <li><span class="font-medium text-base-content">main:</span> Contains the FlyonUI Starter Kit with Qwik, offering a clean and scalable foundation to kickstart your project.</li>
        <li><span class="font-medium text-base-content">components:</span> Showcases practical examples of FlyonUI component usage within a Qwik environment</li>
      </ul>
    </div>
  </div>

  <ul class="timeline timeline-snap-icon timeline-compact timeline-vertical mb-12 w-full ps-0">
    <!-- Installation -->
    <li class="mt-0 mb-0 ps-0">
      <div class="timeline-middle mb-2">
        <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
          1
        </span>
      </div>
      <div class="timeline-end m-0 mb-0 w-full rounded-lg p-4">
        <div class="text-base-content mb-3 font-semibold">Install FlyonUI</div>
        <p>
          Install
          <code>flyonui</code>
          via npm.
        </p>
        {{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}npm i flyonui{{< /code-highlight >}}
      </div>
      <hr class="!w-0.5 rounded-none border-transparent" />
    </li>
    <!-- Add FlyonUI plugin -->
    <li class="mt-0 mb-0 ps-0">
      <div class="timeline-middle mb-2">
        <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
          2
        </span>
      </div>
      <div class="timeline-end m-0 mb-0 w-full rounded-lg p-4">
        <div class="text-base-content mb-3 font-semibold">Add FlyonUI plugin</div>
        <p>Include FlyonUI plugin in your <code>global.css</code> file.</p>
        {{< code-highlight addClass="!mb-0 mt-2" lang="css" >}}// global.css
@import "tailwindcss";
@plugin "flyonui";
@import "flyonui/variants.css";
@source "./node_modules/flyonui/flyonui"; 

/* Import Third-party override css */
/* @import "flyonui/src/vendor/flatpickr.css"; */
/* @import "flyonui/src/vendor/notyf.css"; */
/* @import "flyonui/src/vendor/datatables.css"; */
/* @import "flyonui/src/vendor/editor.css"; */
/* @import "flyonui/src/vendor/fullcalendar.css"; */
/* @import "flyonui/src/vendor/raty.css"; */
/* @import "flyonui/src/vendor/waves.css"; */
/* @import "flyonui/src/vendor/apexcharts.css"; */
{{< /code-highlight >}}
      <p class="!mt-4">
        <strong>Note:</strong> If you want to include specific js component
      </p>
      > **Info:** <span class="font-semibold">Tip :</span> Using specific components helps minimize the size of the generated JavaScript and CSS.
      {{< code-highlight addClass="!mb-0 mt-3" lang="css" >}}// global.css
@source "./node_modules/flyonui/dist/accordion.js" // Specific JS component
{{< /code-highlight >}}
      </div>
      <hr class="!w-0.5 rounded-none border-transparent" />
    </li>
    <!-- Add type definitions for FlyonUI -->
  <li class="mt-0 mb-0 ps-0">
    <div class="timeline-middle mb-2">
      <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
        3
      </span>
    </div>
    <div class="timeline-end mb-0 w-full rounded-lg p-4 m-0">
      <div class="text-base-content mb-3 font-semibold">Add type definitions for FlyonUI</div>
      <p>
        Create the <code>global.d.ts</code> file in the project root directory.
      </p>
      {{< code-highlight addClass="mt-2" lang="react" >}}// global.d.ts
declare global {
  interface Window {
    // Optional third-party libraries
    _;
    $: typeof import("jquery");
    jQuery: typeof import("jquery");
    DataTable;
    Dropzone;

  }
}

export {};
{{< /code-highlight >}}
  </div>
  <hr class="!w-0.5 rounded-none border-transparent" />
  </li>
    <!-- Add the FlyonUI JavaScript -->
    <li class="mt-0 mb-0 ps-0">
      <div class="timeline-middle mb-2">
        <span class="text-base-content flex size-7 items-center justify-center rounded-full border border-base-content/20 font-semibold">
          3
        </span>
      </div>
      <div class="timeline-end m-0 mb-0 w-full rounded-lg p-4">
        <div class="text-base-content mb-3 font-semibold">Add the FlyonUI JavaScript</div>
        <p>Include FlyonUI JavaScript to the <code>root_directory/src/root.tsx</code> file.</p>
        {{< code-highlight addClass="!mb-0 mt-2 max-h-96 highlight-top-rounded-none" lang="react" >}}import { component$ } from "@builder.io/qwik";
import {
  QwikCityProvider,
  ...
} from "@builder.io/qwik-city";

// Optional third-party libraries
import $ from 'jquery';
import _ from 'lodash';
import noUiSlider from 'nouislider';
import 'datatables.net';
import 'dropzone/dist/dropzone-min.js';

window.$ = $;
window._ = _;
window.jQuery = $;
window.DataTable = $.fn.dataTable;
window.noUiSlider = noUiSlider;

...

export default component$(() => {
  return (
    <QwikCityProvider>
      ...
      <body>
        ...
        <script src="../path/to/flyonui/flyonui.js"></script>
      </body>
    </QwikCityProvider>
  );
});{{< /code-highlight >}}

<p class="!mt-4"><strong>Note:</strong> If you want to include specific js component </p>

{{< code-highlight addClass="!mb-0 mt-2 max-h-96 highlight-top-rounded-none" lang="html" >}}
...
<script src="../path/to/flyonui/dist/accordion.js"></script> // Add particular component JS
...
{{< /code-highlight >}}
</div>
</li>

  </ul>
</div>

<h2 class="text-lg font-medium mb-1">Icons</h2>
For icons setup you can refer [Icons](customization/icons/) page.
