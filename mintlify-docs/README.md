# Being Human Studio - Partner Strategy Documentation

Comprehensive partner strategy documentation space for Being Human Studio, including deal structures, partner evaluations, and strategic frameworks.

## Documentation Structure

```
partner-strategy/
├── overview/           # Executive summaries and strategic overviews
├── deal-structures/    # Beach House deals, 5% earnout models
├── evaluations/        # Partner evaluations and assessments
├── frameworks/         # Strategic frameworks and guides
└── tools/             # Partner evaluation tools and resources
```

## Content Included

- **Overview**: 2 executive summaries
- **Deal Structures**: 6 deal structure documents
- **Partner Evaluations**: 4 partner assessments
- **Frameworks & Guides**: 4 strategic frameworks
- **Tools & Resources**: 3 evaluation tools

**Total: 19 partner strategy documents** organized for easy navigation

## Local Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview your documentation changes locally:

```bash
npm i -g mint
```

Run the following command in this directory (where `docs.json` is located):

```bash
mint dev
```

View your local preview at `http://localhost:3000`.

## Deployment to beinghuman.mintlify.app

### Option 1: GitHub Integration (Recommended)

1. Commit and push the mintlify-docs folder to your repository
2. Go to [Mintlify Dashboard](https://dashboard.mintlify.com)
3. Connect your GitHub repository
4. Set the docs directory to `/mintlify-docs` or the appropriate path
5. Mintlify will automatically deploy on every push to main branch

### Option 2: Direct Deploy

```bash
# From this directory
mint deploy
```

Follow the prompts to connect to your Mintlify account.

## MCP Server

Once deployed, your documentation automatically generates an MCP server at:
```
https://beinghuman.mintlify.app/mcp
```

Connect it to Claude Code:
```bash
npx @mintlify/mcp add beinghuman
```

## Configuration

The main configuration is in `docs.json`:
- **Navigation**: Tab and page structure
- **Branding**: Colors, logos, theme
- **Links**: Navbar, footer, social links
- **Features**: MCP, contextual menus, etc.

## Adding New Documentation

1. Create new `.mdx` files in the appropriate `partner-strategy/` subdirectory
2. Add the page path to `docs.json` navigation
3. Test locally with `mint dev`
4. Commit and push (auto-deploys with GitHub integration)

## Troubleshooting

- **Dev environment not running**: Run `mint update` for the latest CLI version
- **Page loads as 404**: Ensure you're in the directory with `docs.json`
- **Navigation issues**: Verify page paths in `docs.json` match file locations

## Resources

- [Mintlify Documentation](https://mintlify.com/docs)
- [Mintlify MCP Guide](https://mintlify.com/docs/ai/model-context-protocol)
- [Being Human Studio GitHub](https://github.com/being-human-studio)
