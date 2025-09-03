# Plonky Agents Catalog - CLI Power Tools

**Total: 56 agents** - Focusați pe CLI puternice și generare de rapoarte/insights

## 🤖 AI-Powered CLI Agents (3)

### claude-code
- **Container**: node:20-bullseye
- **Description**: Anthropic's Claude Code CLI for AI-powered coding
- **Usage**: `ploinky run agent claude-code "refactor this code"`
- **Output**: Code generation, debugging, automated fixes

### gemini-cli  
- **Container**: node:20-bullseye
- **Description**: Google's Gemini CLI with 1M token context
- **Usage**: `ploinky run agent gemini-cli "analyze this error"`
- **Output**: Natural language analysis and solutions

### qwen-code
- **Container**: node:20-bullseye
- **Description**: Alibaba's open-source Qwen Code CLI
- **Usage**: `ploinky run agent qwen-code "implement feature"`
- **Output**: Code generation with 256K-1M context

## 💻 Programming Languages (9)

### python-dev
- **Tools**: pytest, black, flake8, mypy, pylint, jupyter
- **Usage**: `ploinky run agent python-dev pytest --cov`
- **Output**: Test reports, coverage analysis

### node-dev
- **Tools**: typescript, jest, eslint, prettier
- **Usage**: `ploinky run agent node-dev jest --coverage`
- **Output**: Test results, linting reports

### rust-dev
- **Tools**: cargo, rustfmt, clippy, cargo-audit
- **Usage**: `ploinky run agent rust-dev cargo test`
- **Output**: Test results, security audit reports

### go-dev
- **Tools**: gopls, delve, golangci-lint
- **Usage**: `ploinky run agent go-dev go test -cover`
- **Output**: Test coverage, lint analysis

### java-dev
- **Tools**: Maven, Gradle
- **Usage**: `ploinky run agent java-dev mvn test`
- **Output**: JUnit reports, build artifacts

### cpp-dev
- **Tools**: gcc, cmake, clang-format, gdb, valgrind
- **Usage**: `ploinky run agent cpp-dev valgrind ./app`
- **Output**: Memory leak reports, profiling

### php-dev
- **Tools**: PHP 8.3, Composer
- **Usage**: `ploinky run agent php-dev composer test`
- **Output**: PHPUnit results

### ruby-dev
- **Tools**: bundler, rails, rspec, rubocop
- **Usage**: `ploinky run agent ruby-dev rspec`
- **Output**: Test specs, style violations

### dotnet-dev
- **Tools**: .NET 8.0 SDK, Entity Framework
- **Usage**: `ploinky run agent dotnet-dev dotnet test`
- **Output**: Test results, code coverage

## 🗄️ Database CLI Tools (4)

### redis-cli
- **Usage**: `ploinky run agent redis-cli --scan`
- **Output**: Key analysis, memory stats

### postgres-cli
- **Usage**: `ploinky run agent postgres-cli -c "SELECT * FROM pg_stat_activity"`
- **Output**: Query results, performance metrics

### mongodb-cli
- **Usage**: `ploinky run agent mongodb-cli --eval "db.stats()"`
- **Output**: Database statistics, collection info

### database-tools
- **Tools**: PostgreSQL, MySQL, Redis, MongoDB, SQLite clients
- **Usage**: `ploinky run agent database-tools sqlite3 db.sqlite ".schema"`
- **Output**: Schema information, query results

## 🚀 DevOps & Infrastructure (6)

### docker-agent
- **Usage**: `ploinky run agent docker-agent ps -a`
- **Output**: Container status, resource usage

### kubernetes-agent
- **Usage**: `ploinky run agent kubernetes-agent get pods -o wide`
- **Output**: Cluster state, resource allocation

### terraform-agent
- **Usage**: `ploinky run agent terraform-agent plan`
- **Output**: Infrastructure changes report

### ansible-agent
- **Usage**: `ploinky run agent ansible-agent-playbook -C site.yml`
- **Output**: Dry-run changes report

### aws-cli-agent
- **Usage**: `ploinky run agent aws-cli-agent s3 ls --summarize`
- **Output**: AWS resource listings, cost analysis

### vault-agent
- **Usage**: `ploinky run agent vault-agent kv list secret/`
- **Output**: Secret paths, policies audit

## 🧪 Testing & Quality (5)

### testing-tools
- **Tools**: jest, mocha, cypress, playwright, vitest
- **Usage**: `ploinky run agent testing-tools playwright test --reporter=html`
- **Output**: HTML test reports, screenshots

### linting-tools
- **Tools**: eslint, prettier, stylelint, markdownlint
- **Usage**: `ploinky run agent linting-tools eslint . --format json`
- **Output**: JSON lint reports, auto-fixes

### security-scanner
- **Tools**: Trivy
- **Usage**: `ploinky run agent security-scanner fs --severity HIGH .`
- **Output**: Vulnerability reports, CVE listings

### sonarqube
- **Usage**: `ploinky run agent sonarqube -Dsonar.projectKey=myproject`
- **Output**: Code quality metrics, technical debt

### k6-performance
- **Usage**: `ploinky run agent k6-performance run --summary-export=report.json test.js`
- **Output**: Performance metrics, load test results

## 🛠️ Build Tools (3)

### webpack-dev
- **Usage**: `ploinky run agent webpack-dev --analyze`
- **Output**: Bundle analysis, size reports

### vite-dev
- **Usage**: `ploinky run agent vite-dev build --logLevel info`
- **Output**: Build statistics, optimization reports

### esbuild-dev
- **Usage**: `ploinky run agent esbuild-dev --analyze=verbose`
- **Output**: Bundle metrics, tree-shaking report

## 📦 Version Control (2)

### github-cli-agent
- **Usage**: `ploinky run agent github-cli-agent pr list --json`
- **Output**: PR status, CI results

### gitlab-cli-agent
- **Usage**: `ploinky run agent gitlab-cli-agent pipeline list`
- **Output**: Pipeline status, merge requests

## 🌐 Modern JavaScript Runtimes (2)

### deno-runtime
- **Usage**: `ploinky run agent deno-runtime test --coverage`
- **Output**: Test coverage reports

### bun-runtime
- **Usage**: `ploinky run agent bun-runtime test --coverage`
- **Output**: Fast test execution reports

## 🚀 Framework CLIs (7)

### nextjs-dev
- **Usage**: `ploinky run agent nextjs-dev build --debug`
- **Output**: Build analysis, bundle sizes

### remix-dev
- **Usage**: `ploinky run agent remix-dev build --profile`
- **Output**: Build performance metrics

### astro-dev
- **Usage**: `ploinky run agent astro-dev build --verbose`
- **Output**: Static site generation stats

### react-native
- **Usage**: `ploinky run agent react-native bundle --dev false`
- **Output**: Bundle size analysis

### flutter-dev
- **Usage**: `ploinky run agent flutter-dev analyze`
- **Output**: Dart analysis, widget tests

### electron-dev
- **Usage**: `ploinky run agent electron-dev build --publish never`
- **Output**: Build artifacts, app size

### tauri-dev
- **Usage**: `ploinky run agent tauri-dev build --verbose`
- **Output**: Rust + web bundle metrics

## 📡 Message Queues (2)

### kafka-cli
- **Usage**: `ploinky run agent kafka-cli kafka-topics --describe`
- **Output**: Topic configurations, partition info

### rabbitmq-cli
- **Usage**: `ploinky run agent rabbitmq-cli list_queues`
- **Output**: Queue statistics, message counts

## 🛠️ CLI Utilities (7)

### curl-agent
- **Usage**: `ploinky run agent curl-agent -w "@curl-format.txt" -o /dev/null -s URL`
- **Output**: HTTP metrics, response times

### jq-agent
- **Usage**: `ploinky run agent jq-agent '.dependencies | keys' package.json`
- **Output**: JSON transformation, data extraction

### ffmpeg-agent
- **Usage**: `ploinky run agent ffmpeg-agent -i video.mp4 -f null -`
- **Output**: Media file analysis, codec info

### imagemagick
- **Usage**: `ploinky run agent imagemagick identify -verbose image.jpg`
- **Output**: Image metadata, EXIF data

### pandoc-agent
- **Usage**: `ploinky run agent pandoc-agent README.md -t json`
- **Output**: Document AST, format conversion

### postman-cli
- **Usage**: `ploinky run agent postman-cli run collection.json --reporters cli,json`
- **Output**: API test results, response times

### puppeteer-agent
- **Usage**: `ploinky run agent puppeteer-agent screenshot.js`
- **Output**: Page screenshots, performance metrics

## 📊 Data Science (1)

### data-science
- **Tools**: Jupyter, scikit-learn, tensorflow, pytorch
- **Usage**: `ploinky run agent data-science jupyter nbconvert --execute notebook.ipynb`
- **Output**: Executed notebooks, ML model metrics

## 🔧 Documentation (2)

### plantuml-agent
- **Usage**: `ploinky run agent plantuml-agent -tsvg diagram.puml`
- **Output**: UML diagrams, architecture visualizations

### mermaid-cli
- **Usage**: `ploinky run agent mermaid-cli -i diagram.mmd -o output.svg`
- **Output**: Flowcharts, sequence diagrams

## 🌐 Networking (1)

### ngrok-agent
- **Usage**: `ploinky run agent ngrok-agent http 3000 --log stdout`
- **Output**: Tunnel URLs, traffic inspection

## 🔨 System (1)

### BashAgent
- **Usage**: `ploinky run agent BashAgent "find . -type f -exec wc -l {} + | sort -rn"`
- **Output**: Any bash command output

---

## Quick Examples

```bash
# Run security scan
ploinky run agent security-scanner fs .

# Test Python project with coverage
ploinky run agent python-dev pytest --cov --cov-report=html

# Analyze JavaScript bundle
ploinky run agent webpack-dev --analyze

# Check Kubernetes cluster
ploinky run agent kubernetes-agent get all -A

# Performance test
ploinky run agent k6-performance run --vus 10 --duration 30s test.js
```