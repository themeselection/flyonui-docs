# Templates

 A ready-made layout for a document that you can fill in with your own content without needing to worry about formatting.

<!-------------------- What does the Template mean? -------------------->  

## What does the Template mean?

A Template is a pre-designed structure or framework used to create consistent content within a project. It provides a standardized format with placeholders, allowing users to quickly generate new documents or components. Templates save time, ensure uniformity, and make the creation process more efficient.

<!-------------------- How can I access the FlyonUI Templates? -------------------->  

{{< headsingle addClass="!mt-3" level="2" >}} How can I access the FlyonUI Templates? {{< /headsingle >}}

**Step 1: Log In to Your Account**
- Go to <a class="link link-primary" href="https://flyonui.com/">flyonui.com</a> and log in using your credentials.
  
**Step 2: Navigate to the Templates Page**
- Visit the <a class="link link-primary" target="_blank" href="https://flyonui.com/templates">Templates page</a> to explore different types of templates.
    
<img src="https://cdn.flyonui.com/fy-assets/assets/images/templates-image.png" alt="" class="shadow-md rounded-md">  
        
**Step 3: Access the FlyonUI Figma Kit**
- Click the "Get All Access" button to unlock the FlyonUI templates.


<!-------------------- Quick Start -------------------->  

## Quick Start

For <b>Development</b> seamless workflow, instantly view your CSS changes and automatically compile TailwindCSS without any hassle. This ensures a more efficient and streamlined coding experience, allowing you to focus on building while Tailwind handles the rest.

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run dev{{< /code-highlight >}}


For <b>Production</b>, it generates optimized and minified assets, ensuring faster load times and improved performance for deployment. This process refines your code, making it ready for seamless and efficient production use.

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run build:prod{{< /code-highlight >}}

<!-------------------- Folder Structure -------------------->  

## Folder Structure

```text
src/
├── html/
│   ├── dashboard-default/      # Default dashboard layout
├── assets/                     # Build assets and outputs
│   ├── css/                    # Source CSS files
│   │   └── main.css            # Main TailwindCSS source
│   ├── js/                     # JavaScript files
│   ├── img/                    # Images and graphics
│   ├── json/                   # JSON data files
│   ├── dist/                   # Built assets (previously vendor)
│   │   ├── css/                # Compiled CSS
│   │   │   └── output.css      # Generated TailwindCSS output
│   │   ├── js/                 # Built JavaScript
│   │   └── libs/               # External libraries
```

<!-------------------- Commands -------------------->

## Commands
  
<!-- Development Commands -->
### Development Commands
- `pnpm run dev`  - Start TailwindCSS development mode with file watching and local server.
- `pnpm run watch`  - Start TailwindCSS in watch mode (CSS compilation only)
- `pnpm run serve`  - Start a local HTTP server for preview

<!-- Build Commands -->
### Development Commands
- `pnpm run build`  - Build all assets for development
- `pnpm run build:css`  - Compile TailwindCSS without minification
- `pnpm run build:js`  - Copy JavaScript files to dist directory
- `pnpm run build:libs`  - Build external libraries from node_modules
- `pnpm run build:assets`  - Build all assets for development
- `pnpm run build:prod`  - Build all assets for production with minification

<!-------------------- Getting Started -------------------->

## Getting Started

> **Info:** Prerequisites
> <ul>
> <li>Node.js 18.0.0 or higher</li>
> <li>npm or yarn package manager</li>
> </ul>

<!-- Installation -->
### Installation
1. **Install dependencies:** This will install `node_modules` in your file automatically.

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}npm install{{< /code-highlight >}}

2. **Start development:** This will start TailwindCSS in watch mode and compile changes automatically.


{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run dev{{< /code-highlight >}}

3. **Preview your site:** This will start a local server at `http://localhost:8080`

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run dev{{< /code-highlight >}}

<!-------------------- Configuration -------------------->

## Configuration

The main TailwindCSS configuration is defined in the source CSS file at css/main.css. This file uses TailwindCSS 4.x syntax with @import directives and can include custom CSS.

<!-- Build Configuration -->
### Build Configuration

Build settings are managed through a configuration system that controls compilation options, dependencies, environment variables, and build targets for consistency and optimization.

- `package.json` - NPM scripts and dependencies
- `gulpfile.js` - NPM scripts and dependencies
- `build-config.js` - NPM scripts and dependencies
- `libs-build.js` - NPM scripts and dependencies

<!-------------------- How to Third-Party library? -------------------->

## How to Third Party library ?

1. Start by installing the desired library via your terminal or command line interface. You can do this using `npm` or `yarn` as follows: 
```html
npm install nouislider
```
<br>

This will add the library to your `node_modules directory and include it in your package.json dependencies.


2. After installation, verify that the library is present in your `package.json` under the dependencies section, and check that it has been successfully added to the `node_modules` directory.

You can check `package.json` for a corresponding entry:
```html
"dependencies": {
  "nouislider": "~15.8.1"
}
```

3. Next, you'll need to include the library in the `libs-build.js` configuration file. Open this file and add the library to the list of assets in alphabetical order, ensuring that the build process knows to include it in the final output.

For example:
```html
nouislider: {
  src: ['nouislider/dist/nouislider.min.js']
}
```

4. Run the build process to bundle the libraries. Use the following command to trigger the build process:
```html
nr build
```
<br>

This will generate the necessary files and output them into the `assets/dist/libs/` directory. Verify that the `nouislider.min.js` file (or your specific library) is placed correctly within the `assets/dist/libs/` folder.

5. Finally, reference the installed library in your HTML or JavaScript files. Add the corresponding `<script>` tag to your HTML file to include the library from the `assets/dist/libs/` directory.

For example:
```html
<script src="../assets/dist/libs/nouislider/dist/nouislider.min.js"></script>
```
<br>
All Set 🚀
<br>
You’re now ready to use the library in your project!
