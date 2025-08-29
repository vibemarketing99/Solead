# VibeCode - Spec-Driven Development

This project uses spec-workflow for structured development with requirements, design, and task management.

## Local Setup

The spec-workflow tools are installed locally in this project, not globally.

### Available Commands

```bash
# Start dashboard only (standalone mode)
npm run dashboard

# Start MCP server with auto-opening dashboard
npm run dashboard:auto

# Start MCP server only (for use with Claude/Cursor)
npm run mcp

# Show help
npm run spec
```

### Dashboard Access

When running the dashboard, it will be available at:
- **URL**: `http://localhost:3456`
- **Features**: Create steering documents (product.md, tech.md, structure.md), manage specs, track tasks

### MCP Integration

The project is configured to work with:
- **Claude Desktop**: Auto-configured in `~/.config/claude-desktop/claude_desktop_config.json`
- **Cursor**: Auto-configured in `~/.cursor/mcp.json`
- **Local Config**: Project-specific config in `.mcp-config.json`

Both IDE configurations use the local npm installation rather than global npx.

### Steering Documents

Use the steering-guide → create-steering-doc workflow to create:
- `product.md` - Product vision and goals
- `tech.md` - Technical decisions and architecture
- `structure.md` - Codebase organization guidelines

### Spec Workflow

1. **Requirements** → Define what needs to be built
2. **Design** → Plan how to build it
3. **Tasks** → Break down into implementable steps
4. **Implementation** → Execute with progress tracking

All specs are stored in the `/specs` directory (auto-created).

