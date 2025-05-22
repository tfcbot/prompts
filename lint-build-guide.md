# Lint and Build Guide

## Linting Implementation

### 1. Assess Current Setup
- Check for existing lint configurations in the project
- Identify the programming languages and frameworks used
- Review any existing code style guidelines or preferences

### 2. Select Appropriate Linters
- Choose linters compatible with the project's languages and frameworks
- Prioritize industry-standard linters (ESLint for JavaScript/TypeScript, Stylelint for CSS, etc.)
- Consider specialized linters for particular frameworks (React, Vue, etc.)

### 3. Configure Linter Settings
- Create configuration files (.eslintrc, .stylelintrc, etc.) in the project root
- Define rules based on project requirements and team preferences
- Extend recommended configs where appropriate
- Add Zod-specific rules if schema validation is used

### 4. Setup Linting Scripts
- Add lint commands to package.json scripts section:
  ```json
  "scripts": {
    "lint": "eslint . --ext .js,.jsx,.ts,.tsx",
    "lint:fix": "eslint . --ext .js,.jsx,.ts,.tsx --fix",
    "lint:style": "stylelint '**/*.css'",
    "lint:style:fix": "stylelint '**/*.css' --fix"
  }
  ```
- Configure paths and files to ignore (.eslintignore, .stylelintignore)

### 5. Integrate with Development Workflow
- Set up pre-commit hooks using husky/lint-staged to run linting before commits
- Configure editor integrations (VS Code extensions, etc.)
- Document linting workflow in README or contributing guidelines

## Build Process Implementation

### 1. Analyze Project Requirements
- Identify the project type (library, application, server, etc.)
- Determine target environments (browser, Node.js, etc.)
- List performance and optimization requirements

### 2. Select Build Tools
- Choose appropriate bundlers (Bun, webpack, Vite, etc.) based on project needs
- Select transpilers if needed (TypeScript, Babel)
- Determine if additional build steps are required (CSS pre-processing, asset optimization)

### 3. Configure Build Process
- Create configuration files for selected tools (bun.config.js, vite.config.js, etc.)
- Define entry points, output paths, and optimization settings
- Configure environment-specific builds (development, production, staging)

### 4. Setup Build Scripts
- Add build commands to package.json scripts section:
  ```json
  "scripts": {
    "build": "bun build",
    "build:dev": "bun build --dev",
    "build:prod": "bun build --minify"
  }
  ```
- Include any pre-build or post-build steps as needed

### 5. Integrate with Deployment Pipeline
- Configure build artifacts output location
- Document build and deployment process
- Set up CI/CD pipeline integration if applicable

## Implementation Guidelines

1. Prefer Bun over Yarn or npm for package management and building
2. Use Tailwind 3.4.17 if CSS framework is needed (avoid Tailwind v4)
3. Document all commands in the project README
4. Create example commands for common development tasks
5. Keep configuration files as simple as possible while meeting requirements
6. Add detailed comments in configuration files to explain non-standard settings

## Example Implementation

```bash
# Install dependencies
bun add -D eslint eslint-config-standard typescript @typescript-eslint/parser @typescript-eslint/eslint-plugin

# Create configuration files
echo '{
  "extends": ["standard", "plugin:@typescript-eslint/recommended"],
  "parser": "@typescript-eslint/parser",
  "plugins": ["@typescript-eslint"],
  "root": true
}' > .eslintrc.json

# Update package.json
# Add the following to the "scripts" section:
# "lint": "eslint . --ext .js,.jsx,.ts,.tsx",
# "lint:fix": "eslint . --ext .js,.jsx,.ts,.tsx --fix",
# "build": "bun build ./src/index.ts --outdir ./dist",
# "build:dev": "bun build ./src/index.ts --outdir ./dist --dev"
```

Remember to adapt these configurations and commands to the specific needs of your project. Always test lint and build processes thoroughly before committing them to the repository. 