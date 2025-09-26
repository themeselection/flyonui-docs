# Cursor Setup for FlyonUI

Set up Cursor to generate FlyonUI code with Tailwind CSS for fast, efficient web development workflows.


<!-- MCP server -->
## MCP server

<!-- One-Click Install -->
### One-Click Install

If you're using Cursor, the easiest way to set up the Context7 MCP Server is with a single click. Just use the button below to install it instantly.

<a href="https://cursor.com/install-mcp?name=context7&config=eyJjb21tYW5kIjoibnB4IC15IEB1cHN0YXNoL2NvbnRleHQ3LW1jcCJ9" class="btn btn-soft btn-primary no-underline">One-Click Install</a>

<!-- CLI -->
### CLI

Run the following command to install the FlyonUI MCP Server:

```bash
npx install-mcp @upstash/context7-mcp --client cursor
```

<!-- Manual Setup -->
### Manual Setup

 Paste the following configuration into your Cursor MCP config file: `~/.cursor/mcp.json`

```json
{
  "mcpServers": {
    "context7": {
      "command": "npx",
      "args": ["-y", "@upstash/context7-mcp"]
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
