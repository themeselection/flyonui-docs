# Vs Code + Cline Setup for FlyonUI

Configure Cline to seamlessly generate FlyonUI code from your prompts.

<!-- MCP server -->
## MCP server

<!-- CLI -->
### CLI

Run the following command to install the Context7 MCP server:

```bash
npx install-mcp @upstash/context7-mcp --client cline
```

<!-- Manual Setup -->
### Manual Setup


Paste the following configuration into your `cline_mcp_settings.json` file:

```json
{
  "mcpServers": {
    "Context7": {
      "autoApprove": [],
      "disabled": false,
      "timeout": 60,
      "command": "docker",
      "args": ["run", "-i", "--rm", "context7-mcp"],
      "transportType": "stdio"
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
