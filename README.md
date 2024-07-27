# cmd_stash_bundles

cmd_stash_bundles is a repository of curated command bundles designed to enhance your command-line productivity. This repository contains ready-to-use command sets for various technologies, making it easy to manage and deploy commonly used commands in your projects.

## Features

- Technology-Specific Bundles: Access command bundles for a wide range of technologies including AWS, Kubernetes, Docker, Git, and more.
- Seamless Integration: Easily fetch and import command bundles into your cmd_stash setup with a simple CLI command.
- Community Contributions: Contribute your own command bundles to share with the community.

## Getting Started

### Prerequisites

Ensure you have the cmd_stash CLI tool installed and set up in your environment. If you don't have it installed, please refer to the cmd_stash documentation for installation instructions.

### Fetching a Command Bundle

To fetch a command bundle, use the cmd_stash CLI tool with the fetch command:

```bash
cmd_stash fetch <bundle-name>
```

Replace `<bundle-name>` with the name of the bundle you want to fetch. For example, to fetch the bundle for curl, use:

```bash
cmd_stash fetch curl
```

This command will download the specified bundle and import it into your cmd_stash configuration.

### Importing Commands

Fetched commands are automatically imported into your cmd_stash configuration. You don’t need to perform any additional steps to import them.

## Command Bundles

Command bundles are organized by technology and stored in the `bundles` directory. Each technology has its own directory containing a JSON file with the commands.

### Example Directory Structure

```markdown
cmd_stash_bundles/
│
├── git/
│   └── commands.json
├── curl/
│   └── commands.json
├── kubectl/
│   └── commands.json
├── aws/
│   └── commands.json
├── gcp/
│   └── commands.json
├── azure/
│   └── commands.json
├── telnet/
│   └── commands.json
├── scp/
│   └── commands.json
├── docker/
│   └── commands.json
├── tsh/
│   └── commands.json
├── kubernetes/
│   └── commands.json
├── nodejs/
│   └── commands.json
├── react/
│   └── commands.json
├── angular/
│   └── commands.json
├── saltstack/
│   └── commands.json
└── tilt/
    └── commands.json
```

## Adding New Bundles

To contribute new command bundles:

1. Create a New Directory: For each technology, create a new directory under the `bundles` directory.
2. Add Command Files: Add command files in JSON format with the necessary commands.
3. Update `config_gists.yaml`: Add the URLs of your command bundles to the `config_gists.yaml` file to make them accessible via the cmd_stash CLI tool.

### Example JSON File

Here’s an example of what a `commands.json` file might look like:

```json
{
  "aws": {
    "ec2": {
      "list instances": "aws ec2 describe-instances",
      "start instance": "aws ec2 start-instances --instance-ids <instance-id>"
    }
  },
  "kubectl": {
    "pods": {
      "describe pods": "kubectl describe pods",
      "list pods": "kubectl get pods"
    }
  }
}
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions or suggestions, please open an issue on the GitHub repository or contact your-email@example.com.

Feel free to modify this template as needed to better fit your project's specifics.