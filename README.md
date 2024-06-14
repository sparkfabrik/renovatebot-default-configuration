# RenovateBot Default Configuration

RenovateBot is an automated dependency update tool that helps keep your software projects up-to-date by regularly checking for new versions of dependencies and creating pull requests to update them. This README provides an overview of the default configuration used by RenovateBot.

## What is RenovateBot Default Configuration?

RenovateBot's default configuration is a set of predefined settings that determine how the bot behaves when scanning your project's dependencies. These settings are designed to provide a sensible starting point for most projects, while also allowing you to customize and fine-tune the behavior according to your project's specific needs.

## Key Features of Default Configuration

1. **Dependency Types**: The default configuration includes the most common types of dependencies such as npm packages, Python packages, Docker images, and more.

2. **Update Schedule**: RenovateBot is configured to check for updates on a regular basis, usually daily or as specified.

3. **Automated Pull Requests**: When new versions of dependencies are found, RenovateBot creates automated pull requests with the necessary updates. These pull requests can be customized to follow your project's guidelines and coding standards.

4. **Version Pinning**: By default, RenovateBot pins dependencies to the latest version within the specified range, helping to ensure compatibility.

5. **Branch Strategy**: The default configuration often uses a separate branch for each update, allowing for easy testing and review before merging.

6. **Labels and Assignees**: RenovateBot can be configured to add labels and assign specific individuals to the automated pull requests, streamlining the review process.

7. **Customization**: While the default configuration is a great starting point, you can customize many aspects of RenovateBot's behavior, including update frequency, branch naming, commit message formats, and more.

## Getting Started

To use the configurations provided by this repository you can use [shareble config presets](https://docs.renovatebot.com/config-presets/).

All you need to do is add one of the following options to your renovate configuration file (see more info [here](https://docs.renovatebot.com/getting-started/installing-onboarding/#configuration-location)):

**Default config**:

```json
{
  "extends": ["github>sparkfabrik/renovatebot-default-configuration"],
}
```

**Custom config**:

```json
{
  "extends": ["github>sparkfabrik/renovatebot-default-configuration//custom/sparkfabrik"],
}
```

