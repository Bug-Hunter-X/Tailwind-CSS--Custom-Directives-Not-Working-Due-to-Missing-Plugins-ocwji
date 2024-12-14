# Tailwind CSS: Custom Directives Not Working Due to Missing Plugins

This repository demonstrates a common yet easily overlooked issue in Tailwind CSS: the failure of custom directives (like `@apply`) to function correctly due to missing plugins or improper configuration.

## Bug Description
When using custom Tailwind plugins that introduce new directives, it's crucial to ensure the plugin is correctly installed and configured in your `tailwind.config.js` file. Forgetting to include the plugin in the `plugins` array will prevent the custom directives from being processed.

## Bug Reproduction
The `bug.js` file contains a simplified example demonstrating the issue.  The `index.css` file uses a hypothetical custom directive (`@apply`) that's not configured in `tailwind.config.js`, leading to the directive being ignored.

## Solution
The `bugSolution.js` file presents the solution: ensuring the plugin is properly included in the `plugins` array of `tailwind.config.js`.