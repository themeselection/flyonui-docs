# Blocks

Build responsive layouts with FlyonUI Pro Blocks and Tailwind CSS for rapid, professional web development.

<!-------------------- What does the Block mean? -------------------->  

## What does the Block mean?

A Block refers to a segment of pre-designed code, crafted by professional designers and developers to provide reusable components or structures within a project. This modular approach helps streamline the development process, ensuring consistency and efficiency.

<!-- How to use the blocks? -->  

### How to effectively use the blocks?

<iframe class="size-full aspect-video rounded-3xl my-6" src="https://www.youtube.com/embed/kc34UU9Zvm8?si=6Gmut-RaPXpt9BeV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

> For the full blog, check out our post on [dev.to](https://dev.to/themeselection/how-to-use-flyonui-block-with-ai-tools-5b83).

Before getting started, make sure your project is properly set up with FlyonUI. Refer to the official <a class="link link-primary font-semibold"  href="https://flyonui.com/docs/getting-started/quick-start/">Getting Started / Installation docs</a> for setup instructions.

Once your project is ready, you can begin integrating blocks seamlessly.

**Access Pro Blocks:**

FlyonUI offers over **500+ premium blocks and sections**, which you can easily copy and use in your project. Here’s how to access them:

> **Info:** To access the full range of blocks and template code, you can purchase <a class="link link-primary" href="https://flyonui.com/pro#pricing">FlyonUI Pro</a>.

**Step 1: Log In to Your Account**
- Go to <a class="link link-primary" href="https://flyonui.com/">flyonui.com</a> and log in using your credentials.
  
**Step 2: Navigate to the Blocks Page**
- Visit the <a class="link link-primary" target="_blank" href="https://flyonui.com/blocks">Blocks page</a> to explore categories like Marketing, eCommerce, Bento, Datatable, and more.
    
<img src="https://cdn.flyonui.com/fy-assets/assets/images/block-image.webp" alt="block image" class="shadow-md rounded-md">  
        

**Step 3: Select and Copy the Code**
- Choose your desired block (e.g., <a class="link link-primary" target="_blank" href="https://flyonui.com/blocks/marketing-ui/hero-section">Hero Section</a>).
- Click the **Code** tab to view the HTML, CSS, and JavaScript.
- If the block contains a Third-Party badge, setup the mentioned Third-Party package for the code to function properly.
<img src="https://cdn.flyonui.com/fy-assets/assets/images/get-code.webp" alt="get code image" class="shadow-md rounded-md">  
        
- Copy the code and paste it into your project where needed.



<!-- How to modify the blocks? -->  

### How to customize the blocks?

Customizing blocks is easy with TailwindCSS and FlyonUI semantic classes. Here's how you can do it:

1. **Using TailwindCSS**:

   * TailwindCSS provides utility classes to easily adjust the spacing, padding, margins, and other layout properties.
   * For example:

     * **Padding**: You can adjust padding using classes like `p-2`, `p-4` (increasing the padding).

       ```html
       <div class="p-4">
         <!-- Your content goes here -->
       </div>
       ```
     * **Margins**: Similarly, you can adjust margins using classes like `m-2` or `m-4`.

       ```html
       <div class="m-4">
         <!-- Your content goes here -->
       </div>
       ```
     * **Gap**: You can also use the `gap` class to adjust the space between elements within a flex or grid layout.

2. **Using FlyonUI Semantic Classes**:

   * FlyonUI offers predefined classes for common UI elements like buttons and backgrounds.
   * For example:

     * **Change Button Style**: You can change button styles using classes like `btn-primary` to `btn-success` to switch from a default button to a success button.

       ```html
       <button class="btn btn-primary">Primary Button</button>

        To

       <button class="btn btn-success">Success Button</button>
       ```

3. **Update Icons**

   * Blocks use Tabler icons from <a class="link link-primary" target="_blank" href="https://icon-sets.iconify.design/tabler/">Iconify/tabler</a>, but you can also use any other font library of your choice. For more information, refer to the [icon documentation](customization/icons/). 


With these simple tools, you can quickly adjust and style your blocks using both TailwindCSS and FlyonUI classes without needing to write extra CSS.


<!-------------------- What is Copy Prompt? -------------------->  

## How can I use Copy Prompt feature of Block?
The **Copy Prompt** feature in FlyonUI allows you to quickly generate AI-optimized prompts for effortless integration of components/blocks into your project. Click the Copy Prompt button on any component/blocks section. Paste the copied prompt into your preferred IDE like VS Code, Cursor, or Windsurf and append custom instructions such as desired layout, placement context, or target framework conversions. Let the AI editor do the rest. It will automatically convert the copied code into a framework-specific format, making it easy to use in your project.

> **Info:** For the detailed understanding of the copy prompt, refer to the [Copy Prompt](ai-mcp-setup/copy-prompt/) documentation.

<!-------------------- How can I modify FlyonUI block using FlyonUI MCP? -------------------->
## How can I modify FlyonUI block using FlyonUI MCP?
You can easily modify FlyonUI blocks/components using the MCP (MCP Server) by using the `/rui` command. This command allows you to interact with the MCP Server and make changes to the blocks/components as per your requirements.

Example: `/rui Update the layout of hero section from vertical to Horizontal.`

> **Info:** For a basic understanding of the MCP setup and working, refer to the [MCP](pro/mcp/) documentation.

<!-------------------- How to use a block in different frameworks? -------------------->
## How to use a block in different frameworks?

Set up FlyonUI in your chosen framework. For detailed instructions, refer to the [framework integration](pro/mcp/) documentation.

Then, simply use the copy prompt functionality to copy the entire code and, with the help of the AI editor, convert it into a framework-specific format.

```html
<!-- Block Prompt -->
 ....
<!-- /Block Prompt -->

Convert the above code into a React/Vue/Astro component with the correct structure.
```



## Frequently Asked Questions (FAQs)


<div class="accordion divide-neutral/20 divide-y">
  <div class="accordion-item active" id="flyonui-theme">
    <button class="accordion-toggle inline-flex items-center gap-x-4 text-start" aria-controls="flyonui-theme-collapse" aria-expanded="true">
      <span class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
      How can I change the theme ?
    </button>
    <div id="flyonui-theme-collapse" class="accordion-content w-full overflow-hidden transition-[height] duration-300" aria-labelledby="flyonui-theme" role="region">
      <div class="px-5 pb-4">
        <p class="text-base-content/80 font-normal">
     FlyonUI offers a variety of pre-designed themes that allow you to effortlessly transform the appearance of your website. This time-saving feature removes the hassle of selecting color schemes, so you can focus on refining your site’s structure and content while FlyonUI takes care of the design.
      </p>
      <p class="text-base-content/80 font-normal">
        For more details, check out the [Theme docs](customization/themes/).
      </p>
      </div>
    </div>
  </div>

  <div class="accordion-item" id="create-landing-page">
    <button class="accordion-toggle inline-flex items-center gap-x-4 text-start" aria-controls="create-landing-page-collapse" aria-expanded="false">
      <span class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
     How can I create landing page/web page using blocks?
    </button>
    <div id="create-landing-page-collapse" class="accordion-content hidden w-full overflow-hidden transition-[height] duration-300" aria-labelledby="create-landing-page" role="region">
      <div class="px-5 pb-4">
        <p class="text-base-content/80 font-normal">
        FlyonUI Pro blocks provide a wide selection of professionally designed blocks, each with a well-organized layout and structure. Simply select the blocks you need for your website and copy-paste them in sequence based on your requirements.
      </p>
      <p class="text-base-content/80 font-normal">
        Additionally, with FlyonUI MCP, you can easily customize these blocks to suit your specific needs. For more information, check out the [MCP docs](pro/mcp/).
      </p>
      </div>
    </div>
  </div>
</div>
