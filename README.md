# Documentation Template

<div align="center">
  <img src="../images/logo.png" alt="Dangelmaiers Logo" width="80" height="80">
  <h3 align="center">doc-template</h3>
  <p align="center">
    Standard template for documentation repositories in the Dangelmaiers organization
    <br />
    <a href="#about"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#usage">View Usage</a>
    &middot;
    <a href="https://github.com/Dangelmaiers/doc-template/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/Dangelmaiers/doc-template/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about">About</a></li>
    <li><a href="#documentation-context">Documentation Context</a></li>
    <li><a href="#repository-structure">Repository Structure</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#naming-conventions">Naming Conventions</a></li>
    <li><a href="#documentation-standards">Documentation Standards</a></li>
    <li><a href="#cross-referencing">Cross-Referencing</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About

This repository serves as a template for all documentation repositories in the Dangelmaiers organization. It follows standardized naming conventions and includes required files and directory structures for consistent documentation across the organization's infrastructure and services.

### Documentation Types and Tags

Depending on the documentation category, add relevant tags:

- `infrastructure`: Proxmox and infrastructure documentation
- `containers`: Container service documentation
- `maintenance`: Maintenance procedures
- `reference`: Reference documentation and standards

## Documentation Context

Documentation repositories in the Dangelmaiers organization serve to:

- Provide comprehensive documentation for infrastructure components
- Document container service configurations and usage
- Standardize maintenance procedures
- Establish cross-referencing between related systems
- Create a single source of truth for organizational knowledge

## Repository Structure

All documentation repositories follow this standard structure:

```
doc-*/
├── README.md                # Overview and documentation index
├── guides/                  # User and implementation guides
│   └── README.md            # Guide structure and organization
├── maintenance/             # Maintenance procedures
│   └── README.md            # Maintenance documentation guidelines
└── _templates/              # Documentation templates
    └── standard-doc.md      # Standard document template
```

## Usage

To use this template for a new documentation repository:

1. Create a new repository using this template
2. Rename according to the `doc-*` convention (e.g., `doc-infrastructure`, `doc-containers`)
3. Update the README.md with specific focus and context
4. Create appropriate guide documents in the `guides/` directory
5. Add maintenance procedures in the `maintenance/` directory
6. Use templates from `_templates/` for new documents

## Naming Conventions

The Dangelmaiers organization uses the following prefix system:

- `pve-*`: Proxmox Virtual Environment related repositories
- `lxc-*`: Container specific configurations and setups
- `doc-*`: Documentation repositories

Examples of documentation repository names:
- `doc-infrastructure`: Infrastructure documentation
- `doc-containers`: Container setup guides
- `doc-maintenance`: Maintenance procedures

## Documentation Standards

### File Format

- Use Markdown (`.md`) for all documentation
- Begin each document with a clear title using `# Title`
- Include a table of contents for documents longer than 3 sections
- Use relative links for cross-referencing within the organization

### Content Structure

Each document should include:

1. **Introduction/Overview** - What the document covers
2. **Prerequisites** - What is needed before proceeding
3. **Main Content** - Organized in logical sections
4. **Troubleshooting** - Common issues and solutions
5. **References** - Links to related documentation

### Writing Style

- Use clear, concise language
- Write in the present tense
- Use active voice where possible
- Include examples and code snippets
- Add screenshots or diagrams for complex procedures

## Cross-Referencing

### Internal References

Link to other documents within the same repository using relative paths:

```markdown
See the [installation guide](guides/installation.md) for setup instructions.
```

### Cross-Repository References

Link to documents in other repositories using absolute GitHub URLs:

```markdown
For network configuration, refer to the [network setup](https://github.com/Dangelmaiers/pve-network/blob/main/SETUP.md) documentation.
```

### Reference Mapping

Maintain a reference map in each repository that documents connections to other repositories:

```markdown
## Related Repositories

- [pve-core](https://github.com/Dangelmaiers/pve-core) - Core Proxmox configuration
- [lxc-grafana](https://github.com/Dangelmaiers/lxc-grafana) - Monitoring dashboards
```

## Contributing

Contributions should follow the Dangelmaiers organization standards:

1. Fork the repository
2. Create a documentation branch (`git checkout -b docs/improvement`)
3. Commit your changes (`git commit -m 'Add documentation for XYZ'`)
4. Push to the branch (`git push origin docs/improvement`)
5. Open a pull request

## License

Refer to the `LICENSE.txt` file for license information.

## Contact

Documentation Team - docs@dangelmaiers.org

---

*This repository follows the Dangelmaiers organization structure standards. For more information, refer to the [doc-maintenance](https://github.com/Dangelmaiers/doc-maintenance) repository.*

