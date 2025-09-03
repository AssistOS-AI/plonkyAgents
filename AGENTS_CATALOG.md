# Plonky Agents Catalog

## AI-Powered CLI Agents

### claude-code
- **Container**: node:20-bullseye
- **Description**: Anthropic's Claude Code CLI for AI-powered coding assistance
- **Run Command**: `ploinky run agent claude-code`
- **Features**: Code generation, debugging, file management, project automation

### gemini-cli  
- **Container**: node:20-bullseye
- **Description**: Google's Gemini CLI with 1M token context window
- **Run Command**: `ploinky run agent gemini-cli`
- **Features**: Natural language commands, ReAct loop, MCP servers support

### qwen-code
- **Container**: node:20-bullseye
- **Description**: Alibaba's open-source Qwen Code CLI
- **Run Command**: `ploinky run agent qwen-code`
- **Features**: 256K-1M token context, workflow automation, privacy-focused

## Programming Languages

### python-dev
- **Container**: python:3.11-bullseye
- **Description**: Python development environment with common tools
- **Run Command**: `ploinky run agent python-dev`
- **Tools**: pytest, black, flake8, mypy, pylint, jupyter, pandas, numpy, flask, django, fastapi

### node-dev
- **Container**: node:20-bullseye
- **Description**: Node.js/TypeScript development environment
- **Run Command**: `ploinky run agent node-dev`
- **Tools**: typescript, ts-node, jest, mocha, eslint, prettier, webpack, vite

### rust-dev
- **Container**: rust:1.75-bullseye
- **Description**: Rust development environment
- **Run Command**: `ploinky run agent rust-dev`
- **Tools**: cargo, rustfmt, clippy, cargo-watch, cargo-audit

### go-dev
- **Container**: golang:1.21-bullseye
- **Description**: Go development environment
- **Run Command**: `ploinky run agent go-dev`
- **Tools**: gopls, delve debugger, golangci-lint

### java-dev
- **Container**: maven:3.9-openjdk-17
- **Description**: Java development with Maven and Gradle
- **Run Command**: `ploinky run agent java-dev`
- **Tools**: Maven, Gradle, OpenJDK 17

### cpp-dev
- **Container**: gcc:13
- **Description**: C/C++ development environment
- **Run Command**: `ploinky run agent cpp-dev`
- **Tools**: gcc, g++, cmake, clang-format, gdb, valgrind

### php-dev
- **Container**: php:8.3-cli
- **Description**: PHP development environment
- **Run Command**: `ploinky run agent php-dev`
- **Tools**: PHP 8.3, Composer

### ruby-dev
- **Container**: ruby:3.3
- **Description**: Ruby development environment
- **Run Command**: `ploinky run agent ruby-dev`
- **Tools**: bundler, rails, rspec, rubocop, pry

### dotnet-dev
- **Container**: mcr.microsoft.com/dotnet/sdk:8.0
- **Description**: .NET development environment
- **Run Command**: `ploinky run agent dotnet-dev`
- **Tools**: .NET 8.0 SDK, Entity Framework, dotnet-format

## Testing & Quality

### testing-tools
- **Container**: node:20-bullseye
- **Description**: JavaScript testing frameworks
- **Run Command**: `ploinky run agent testing-tools`
- **Tools**: jest, mocha, chai, cypress, playwright, vitest

### linting-tools
- **Container**: node:20-bullseye
- **Description**: Code linting and formatting tools
- **Run Command**: `ploinky run agent linting-tools`
- **Tools**: eslint, prettier, stylelint, htmlhint, markdownlint, biome

### security-scanner
- **Container**: aquasec/trivy:latest
- **Description**: Security vulnerability scanning
- **Run Command**: `ploinky run agent security-scanner`
- **Tools**: Trivy, nmap, nikto

## DevOps & Infrastructure

### docker-agent
- **Container**: docker:24-cli
- **Description**: Docker CLI for container management
- **Run Command**: `ploinky run agent docker-agent`
- **Features**: Docker commands, container management

### kubernetes-agent
- **Container**: bitnami/kubectl:latest
- **Description**: Kubernetes cluster management
- **Run Command**: `ploinky run agent kubernetes-agent`
- **Tools**: kubectl, helm

### terraform-agent
- **Container**: hashicorp/terraform:1.6
- **Description**: Infrastructure as Code with Terraform
- **Run Command**: `ploinky run agent terraform-agent`
- **Features**: Terraform CLI for infrastructure provisioning

### aws-cli-agent
- **Container**: amazon/aws-cli:latest
- **Description**: AWS cloud management
- **Run Command**: `ploinky run agent aws-cli-agent`
- **Features**: Full AWS CLI capabilities

## Version Control & Collaboration

### github-cli-agent
- **Container**: ghcr.io/cli/cli:latest
- **Description**: GitHub CLI for repository management
- **Run Command**: `ploinky run agent github-cli-agent`
- **Features**: PR management, issues, releases

### gitlab-cli-agent
- **Container**: alpine:latest
- **Description**: GitLab CLI for project management
- **Run Command**: `ploinky run agent gitlab-cli-agent`
- **Features**: GitLab project and CI/CD management

## Data & Analytics

### data-science
- **Container**: jupyter/datascience-notebook:latest
- **Description**: Data science and ML environment
- **Run Command**: `ploinky run agent data-science`
- **Tools**: Jupyter Lab, scikit-learn, tensorflow, pytorch, transformers

### database-tools
- **Container**: ubuntu:22.04
- **Description**: Database client tools
- **Run Command**: `ploinky run agent database-tools`
- **Tools**: PostgreSQL, MySQL, Redis, MongoDB, SQLite clients

## System & Monitoring

### monitoring-agent
- **Container**: prom/prometheus:latest
- **Description**: System monitoring tools
- **Run Command**: `ploinky run agent monitoring-agent`
- **Tools**: Prometheus, htop, iotop, iftop

### BashAgent
- **Container**: mcr.microsoft.com/devcontainers/base:debian
- **Description**: Basic bash environment
- **Run Command**: `ploinky run agent BashAgent`
- **Features**: Standard bash shell with basic utilities

## Usage Examples

### Running an AI coding assistant:
```bash
ploinky run agent claude-code "Help me refactor this code"
ploinky run agent gemini-cli "Debug this error"
```

### Python development:
```bash
ploinky run agent python-dev
# Inside container:
python script.py
pytest tests/
black .
```

### Running tests:
```bash
ploinky run agent testing-tools jest
ploinky run agent python-dev pytest
```

### Security scanning:
```bash
ploinky run agent security-scanner fs .
ploinky run agent security-scanner image myapp:latest
```

### Interactive shell:
```bash
ploinky run bash python-dev  # Get bash shell in Python container
ploinky run bash node-dev     # Get bash shell in Node container
```

## Environment Variables

To use API keys with AI agents, configure them in `.ploinky/.secrets`:
```bash
ploinky add env ANTHROPIC_API_KEY "your-key"
ploinky enable env claude-code ANTHROPIC_API_KEY

ploinky add env OPENAI_API_KEY "your-key"  
ploinky enable env gemini-cli OPENAI_API_KEY
```

## Updating Agents

Update agent software:
```bash
ploinky run update claude-code
ploinky run update python-dev
```