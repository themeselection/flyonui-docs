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
    
<img src="https://cdn.flyonui.com/fy-assets/assets/images/templates-image.png" alt="templates pages" class="shadow-md rounded-md">  

**Step 3: Download the Templates(.zip)**
- Click the "Download" button to get the .zip file and extract the file.

> **Info:** Once you have downloaded and extracted the template ZIP file, you can follow the instructions below to set up and use the templates in your project.

<!-------------------- Folder Structure -------------------->  

## Folder Structure

```text
**Template Name**/
├── html/
│   ├── ...../                  # Folder 
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
<!-------------------- Getting Started -------------------->

## Getting Started

> **Info:** Prerequisites
> <ul>
> <li>Node.js 18.0.0 or higher</li>
> <li>npm or yarn package manager</li>
> </ul>

If you do not have pnpm installed, follow the steps below to get started:
1. **Install Node.js**(if not already installed): Visit <a class="link link-primary" href="https://nodejs.org/en" target="_blank">Node.js website</a>  and download the latest LTS version.

2. **Install pnpm**: Run the following command in your terminal:
{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}npm install -g pnpm{{< /code-highlight >}}

<!-- Installation -->  
### Installation
1. **Install dependencies:** This will install `node_modules` in your file automatically.

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm install{{< /code-highlight >}}

2. **Start development:** This will start TailwindCSS in watch mode and compile changes automatically.


{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run build{{< /code-highlight >}}

3. **Preview your site:** This will start a local server at `http://localhost:8080`

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run serve{{< /code-highlight >}}
<br>
**OR**

3. **Start Development:** This will start TailwindCSS in watch mode and compile changes automatically.

{{< code-highlight addClass="!mb-0 mt-2" lang="bash" >}}pnpm run dev{{< /code-highlight >}}
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

<!-------------------- Configuration -------------------->

## Configuration

The main TailwindCSS configuration is defined in the source CSS file at `css/main.css`. This file uses TailwindCSS 4.x syntax with `@import` directives and can include custom CSS.

<!-- Build Configuration -->
### Build Configuration

Build settings are managed through a configuration system that controls compilation options, dependencies, environment variables, and build targets for consistency and optimization.

- `package.json`
- `gulpfile.js`
- `build-config.js`
- `libs-build.js`

<!-------------------- How to Add Third-Party library? -------------------->

## How to Add Third Party library ?

1. Start by installing the desired library via your terminal or command line interface. You can do this using `npm` or `yarn` as follows: 
```html
pnpm install nouislider
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
pnpm run build
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
