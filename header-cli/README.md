# header-cli

A simple CLI utility for generating formatted text headers.

## 📦 Requirements

* Python >= 3.9

## 🛠 Usage

Run with a positional argument: 

```console
$ header "project title"
################################ - project title - #################################
```

Run with flags:
```console
$ header --head "build complete" --style multi --char "=" --width 60 -upper
============================================================
= - BUILD COMPLETE - 
============================================================
```

### ⚙️ Options

`header-cli` supports the following flags:

| Flag | Description | Default |
|------|-------------|---------|
| `head` (positional) | Header text | — |
| `-H, --head` | Header text (alternative flag form) | — |
| `-s, --style` | Border style (`single`, `multi`) | `single` |
| `-c, --char` | Character to use for the border | `#` |
| `-w, --width` | Width of the rows | `84` |
| `-C, --case` | Case of the header | `upper` |

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/utils.git
cd utils/header
```

### Unix

Make files executable:

```bash
chmod +x header
```

Additionally, you can copy any app to a location in your PATH:

```bash
cp header ~/.local/bin/header
```

### Windows

Copy `header` to a location of your choice. Then, create a batch file to call it from the terminal:

e.g. `header.bat`:
```cmd
@echo off
python C:\path\to\header %*
```
Then, copy `header.bat` to a location in your PATH.
