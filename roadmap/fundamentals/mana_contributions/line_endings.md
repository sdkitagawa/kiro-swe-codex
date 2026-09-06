# CRLF, CR, LF line endings

`CR` and `LF` are control characters. They are used to mark a line break (new line) in a text file.
- Windows uses a two character sequence, `CR LF`.
- Unix and Linux (as well as macOS starting with macOS X 10.0) only use `LF`.
- The classic Mac OS (before 10.0) used `CR`.

`CR` stands for **Carriage Return**. `LF` stands for **Line Feed**. These two expressions have their roots in the old typewriters and teletypewriters (TTY).

- `LF` moved the paper up, but kept the horizontal position identical.
- `CR` brought back the "carriage", so that the next character typed would be at the leftmost position on the paper, but on the same line.
- `CR` + `LF` was doing both, preparing to type a new line.

As time went by, the physical semantics of the codes were not applicable, and as memory and floppy disk space were at a premium, some OS designers decided to only use one of the characters.

Most modern text editors and text-oriented applications offer options and settings that allow the automatic detection of the file's end-of-line convention and to display it accordingly.

Git technology uses `LF` line endings, because Git runs on Linux. When you clone a repository to your PC, if you are using Windows OS, the files will be converted to `CRLF` so your PC can read them properly.
When you commit and push the files to the repository, they'll be converted back to `LF`.

`LF will be replaced by CRLF the next time Git touches it.` ➟ If you are using Windows OS, to avoid receiving a warning like this one, make sure to leave one empty line (a new line) at the end of the file you are committing.

However, having `CRLF` files in the repository shouldn't be an issue most of the time.

There are two scenarios where it might become an issue:

1) You're executing some code in `WSL` (Windows Subsystem for Linux) or Linux; `CRLF` can sometimes cause problems because Linux expects `LF`.
2) Other collaborators on the repository might be using Linux, which will need `LF`.
