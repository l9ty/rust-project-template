# Rust project template

## Quick Start

```shell
cargo generate -g https://github.com/l9ty/rust-project-template.git
cd $PROJECT_ROOT
# edit cliff.toml: `postprocessors = { replace = $PROJECT_REPO }`
pre-commit install
```


## 环境配置

### VSCode 插件

- rust-analyzer: Rust 语言支持
- Rust Test lens: Rust 测试支持
- Rust Test Explorer: Rust 测试概览
- crates: Rust 包管理
- Even Better TOML: TOML 文件支持

- Better Comments: 优化注释显示
- Error Lens: 错误提示优化
- GitLens: Git 增强
- Github Copilot: 代码提示
- indent-rainbow: 缩进显示优化
- Prettier - Code formatter: 代码格式化
- REST client: REST API 调试
- TODO Highlight: TODO 高亮
- YAML: YAML 文件支持
- vscode-icons: 图标优化

### cargo config

cargo 全局配置 `~/.cargo/config.toml`

```toml
[build]
target-dir = ".target"
# cargo install sccache
rustc-wrapper = ".cargo/bin/sccache"
```

### 安装 cargo generate

cargo generate 是一个用于生成项目模板的工具。它可以使用已有的 github repo 作为模版生成新的项目。

```bash
cargo install cargo-generate
```

```bash
cargo generate l9ty/rust-project-template
```

### 安装 pre-commit

pre-commit 是一个代码检查工具，可以在提交代码前进行代码检查。

```bash
pipx install pre-commit
# debian: apt install pre-commit
```

安装成功后运行 `pre-commit install` 即可。

### 安装 Cargo deny

Cargo deny 是一个 Cargo 插件，可以用于检查依赖的安全性。

```bash
cargo install cargo-deny
```

### 安装 typos

typos 是一个拼写检查工具。

```bash
cargo install typos-cli
```

### 安装 git cliff

git cliff 是一个生成 changelog 的工具。

```bash
cargo install git-cliff
```

### 安装 cargo nextest

cargo nextest 是一个 Rust 增强测试工具。

```bash
cargo install cargo-nextest
```
