# Playwright Project with MCP Support

This project is set up with Playwright for browser automation and testing, along with Model Context Protocol (MCP) support.

## Installation

The project is already set up with the following packages:
- `@playwright/test` - Playwright testing framework
- `playwright` - Playwright browser automation
- `@playwright/mcp` - Playwright MCP server

## Running Tests

### Basic Test Commands

```bash
# Run all tests
npm test

# Run tests in headed mode (visible browser)
npm run test:headed

# Run tests with UI mode
npm run test:ui

# Run tests in debug mode
npm run test:debug

# Show test report
npm run report
```

### Using Playwright MCP

The `@playwright/mcp` package provides Model Context Protocol support for Playwright, allowing AI assistants to interact with browsers programmatically.

To use the MCP server:

1. **Start the MCP server:**
   ```bash
   npx @playwright/mcp
   ```

2. **Configure your MCP client** to connect to the Playwright MCP server.

3. **Use the MCP tools** to:
   - Navigate to web pages
   - Interact with page elements
   - Take screenshots
   - Extract page content
   - Perform browser automation tasks

## Project Structure

```
├── tests/                 # Test files
│   └── example.spec.ts   # Sample test
├── playwright.config.ts  # Playwright configuration
├── tsconfig.json         # TypeScript configuration
├── package.json          # Project dependencies and scripts
└── README.md            # This file
```

## Configuration

The `playwright.config.ts` file is configured with:
- HTML reporter for test results
- Support for Chromium, Firefox, and WebKit browsers
- Parallel test execution
- Trace collection on retry

## Writing Tests

Tests are written in TypeScript and use the Playwright testing framework. See `tests/example.spec.ts` for a basic example.

## Browser Support

The project supports:
- Chromium (Chrome/Edge)
- Firefox
- WebKit (Safari)

Browsers are automatically downloaded when you first run the tests.

## MCP Integration

The Playwright MCP server allows AI assistants to:
- Control browsers programmatically
- Navigate web pages
- Interact with DOM elements
- Capture screenshots and videos
- Extract page content
- Perform complex browser automation tasks

This makes it easy to integrate browser automation into AI-powered workflows and applications.
