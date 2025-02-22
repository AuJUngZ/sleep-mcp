# Sleep MCP Server

<img src="assets/sleep-logo.png" width="256" alt="Sleep MCP Logo" />

A Model Context Protocol (MCP) server that provides a simple sleep/wait tool. Useful for adding delays between operations, such as waiting between API calls or testing eventually consistent systems.

## Available Tools

- `sleep`: Wait for a specified duration in milliseconds

## Installation

```bash
git clone [repository-url]
npm install
```

## Configuration

Add to your Cline MCP settings file (ex. ~/.config/Code/User/globalStorage/saoudrizwan.claude-dev/settings/cline_mcp_settings.json):

```json
{
  "mcpServers": {
    "sleep": {
      "command": "node",
      "args": ["/path/to/sleep-server/build/index.js"],
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

## Development

### Setting Up Tests

The tests verify the sleep functionality with various durations:

```bash
npm test
```

### Building

```bash
npm run build
```

## License

MIT
