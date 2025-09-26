# Windsurf Setup for FlyonUI

Set up Windsurf to generate FlyonUI code with Tailwind CSS for fast, efficient web development workflows.

<!-- MCP server -->
## MCP server

<!-- CLI -->
### CLI

Run the following command to install the Context7 MCP server:

```bash
npx install-mcp @upstash/context7-mcp --client windsurf
```

<!-- Manual Setup -->
### Manual Setup

Add the following configuration to your Windsurf MCP config file: `~/.codeium/windsurf/mcp_config.json`

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
