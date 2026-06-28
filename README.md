# Walker
Walker is a small program to build complete HTML pages in an output folder using a template and an input folder of Mardown pages. 

The first line of an input file is used as a page title, replacing the `[TITLE]` token in the template. The rest of the file replaces the `[CONTENT]` token.

## Install

Executable files are located in the releases section. Download the .exe file if you are on Windows and the un-extended file
if you are on Linux or macOS. Run as you would a normal comamnd in your terminal. You may have to give the file
executable permissions (Using `chmod +x` on Linux/macOS or the "Run as Administrator" function on Windows).
  
If neither file runs on your system, you can build a new one using Go. Install the Go langauge on your system from
[go.dev](https://go.dev). Clone this repository and then run `go build` while in the folder to make a new executable
for your system's architecture and operating system.

## Usage

To learn Walker, simply use the `-h` flag. Which prints...

  ```
    Usage of .\walker.exe:
      -i string
        Input folder of Markdown files (default: "src")
      -o string
        Output folder to place complete HTML pages. This folder is created if it doesn't exist. Existing *.html files, *.htm files, and empty subdirectories in here are deleted! (default "docs")
      -t string
        Template HTML page to inject converted Markdown into (default "template.html")
  ```

## Example website(s)

- [karlramberg.com](https://github.com/karlramberg/karlramberg.com)
