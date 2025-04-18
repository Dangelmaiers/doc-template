
# Documentation Guides

This document outlines the standard structure and best practices for creating guides in the Dangelmaiers organization documentation repositories.

## Guide Structure

All guides should be organized in the `guides/` directory following this structure:

```
guides/
├── README.md                # This file
├── setup/                   # Setup guides
│   ├── installation.md      # Installation procedures
│   ├── configuration.md     # Configuration guides
│   └── integration.md       # Integration instructions
├── usage/                   # Usage guides
│   ├── basic-usage.md       # Basic usage instructions
│   ├── advanced-usage.md    # Advanced usage scenarios
│   └── examples.md          # Usage examples
└── troubleshooting/         # Troubleshooting guides
    ├── common-issues.md     # Common issues and solutions
    ├── diagnostics.md       # Diagnostic procedures
    └── recovery.md          # Recovery procedures
```

## Types of Guides

### Setup Guides

Setup guides focus on the initial implementation of services and systems:

- **Installation Guides** - Step-by-step instructions for installing software or setting up infrastructure
- **Configuration Guides** - Detailed information on configuring services
- **Integration Guides** - Instructions for integrating services with other systems

### Usage Guides

Usage guides explain how to use the implemented services:

- **Basic Usage** - Fundamental operations and commands
- **Advanced Usage** - Complex scenarios and advanced features
- **Examples** - Real-world examples and use cases

### Troubleshooting Guides

Troubleshooting guides help diagnose and resolve issues:

- **Common Issues** - Frequently encountered problems and their solutions
- **Diagnostics** - Procedures for identifying the root cause of problems
- **Recovery** - Steps to recover from failures or errors

## Best Practices for Writing Guides

### Content Organization

1. **Follow the Template** - Use the [standard-doc.md](../_templates/standard-doc.md) template
2. **Progressive Disclosure** - Start with basic information before advanced topics
3. **Logical Flow** - Organize content in a logical sequence
4. **Consistent Structure** - Maintain consistent headings and formatting

### Writing Style

1. **Clear Instructions** - Write clear, actionable instructions
2. **Step-by-Step Format** - Number steps for procedures
3. **Command Examples** - Include specific command examples
4. **Expected Output** - Show expected output of commands when relevant

Example of good step formatting:

```markdown
1. Connect to the server:
   ```sh
   ssh user@server-address
   ```

2. Navigate to the configuration directory:
   ```sh
   cd /etc/service/
   ```

3. Edit the configuration file:
   ```sh
   nano config.yml
   ```
```

### Visual Elements

1. **Screenshots** - Include screenshots for complex UI operations
2. **Diagrams** - Use diagrams to explain complex architectures or workflows
3. **Callouts** - Use blockquotes for important notes or warnings

Example of a good callout:

```markdown
> **Warning:** This operation will delete all data. Make sure to create a backup first.
```

### Code and Configuration Examples

1. **Syntax Highlighting** - Use markdown code fences with appropriate language tags
2. **Complete Examples** - Provide complete, working examples
3. **Explanatory Comments** - Include comments to explain code or configuration

Example of good code formatting:

```markdown
```yaml
# Main service configuration
service:
  # The port the service will listen on
  port: 8080
  
  # Authentication settings
  auth:
    enabled: true
    provider: local
```
```

## Guide Naming Conventions

Use descriptive, hyphenated names for guide files:

- `installation-proxmox.md`
- `configure-network-bridges.md`
- `troubleshoot-database-connection.md`

## Updating Guides

When updating guides:

1. Update the "Last Updated" date in the document metadata
2. Increment the version number
3. Add a note about significant changes at the beginning of the document
4. Consider maintaining a change log for major documents

---

*This document follows the Dangelmaiers organization documentation standards. For questions or issues, contact the documentation team.*

