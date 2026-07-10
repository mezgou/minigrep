# minigrep

A minimal, dependency-free command-line text search tool written in Rust

It reads a UTF-8 file and prints every line containing the given text

## Usage

Pass the text to search for followed by the file path

```bash
cargo run -- nobody ./data/poem.txt
```

This searches `./data/poem.txt` for `nobody`

Output

```text
Searching for nobody
In file ./data/poem.txt
I'm nobody! Who are you?
Are you nobody, too?
```

Search is case-sensitive by default

Enable case-insensitive search with `CASE_INSENSITIVE`

```bash
CASE_INSENSITIVE=1 cargo run -- ARE ./data/poem.txt
```

Wrap queries and file paths that contain spaces in quotes

## License

Licensed under the [MIT License](LICENSE)
