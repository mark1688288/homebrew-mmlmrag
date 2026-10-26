# homebrew-mmlmrag

Homebrew tap for [mmlmRAG](https://github.com/mark1688288/mmlmRAG).

## Install

```bash
brew install mark1688288/mmlmrag/mmlmrag
```

This installs the `rag` command. The formula depends on macOS and `python@3.13`. Its Python resources are the Apple Silicon wheels for tag `v0.1.0`. The first `rag` command creates `~/.mmlmrag`, including a private environment and, when absent, `rag.toml`. A `rag.toml` in the working directory or a parent is used instead.

Ollama stays separate:

```bash
brew install ollama
brew services start ollama
rag models pull
```

In a `Brewfile`:

```ruby
tap "mark1688288/mmlmrag"
brew "mmlmrag"
```
