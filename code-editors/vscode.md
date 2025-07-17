# VS Code Setup for FlyonUI

Configure VS Code to seamlessly generate FlyonUI code from your prompts.

<!-- MCP server -->
## MCP server

<!-- One-Click Install -->
### One-Click Install

If you're using VS Code, the easiest way to set up the Context7 MCP Server is with a single click. Just use the button below to install it instantly.

<a href="https://insiders.vscode.dev/redirect?url=vscode%3Amcp%2Finstall%3F%7B%22name%22%3A%22context7%22%2C%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22%40upstash%2Fcontext7-mcp%40latest%22%5D%7D" class="btn btn-soft btn-primary no-underline">One-Click Install</a>

<!-- Manual Setup -->
### Manual Setup

Open the `mcp.json` file in your user profile by running the `MCP: Open User Configuration` command from the Command Palette.


```json
{
  "mcp": {
    "servers": {
     "Context7": {
       "command": "npx",
       "args": ["-y", "@upstash/context7-mcp@latest"]
     }
    }
  }
}
```

<br>

<!-- Usage -->
### Usage


Now in `Agent Mode`, you can ask AI anything about FlyonUI. Start your prompt with `use context7`.

For example:

```html
Use context7, and create me a FAQ for my project using FlyonUI accordion shadow example.
```
<br>

```html
use context7, Create me Registration where in Password use togglepPassword component from flyonui.
```
