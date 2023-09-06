# Media Batch Renamer (mbr)

Media Batch Renamer (mbr) is a command-line script written in Bash that allows you to organize and rename media files in batches. It utilizes the `mediainfo` command-line tool to extract metadata information from media files and provides customizable options for renaming and organizing them.

## Features

- Extracts metadata information using `mediainfo`.
- Renames media files based on metadata (e.g., movie name, recorded year, TV show details).
- Organizes media files into directory structures based on customizable patterns.
- Supports batch processing of multiple media files.
- Provides options for recursive or non-recursive file searching.
- Customizable output directory and filename formats.
- Verbose mode for detailed output during processing.

## Prerequisites

- `mediainfo` command-line tool: Ensure that `mediainfo` is installed on your system. You can install it using package managers such as `apt` or `brew`.

## Usage

1. Clone the repository or download the "mbr" script directly.
2. Make the script executable: `chmod +x mbr`
3. Run the script with the desired options:

```bash
./mbr [-v|--verbose] [-r|--recursive] [-o|--output] [-n|--no-folders] [-h|--help]
```

Options:

- `-v` or `--verbose`: Enable verbose mode for detailed output during processing.
- `-r` or `--recursive`: Perform a recursive search for media files within subdirectories.
- `-o` or `--output`: Specify the output directory for the organized files. By default, it uses the current directory.
- `-n` or `--no-folders`: Prevent creating separate directories for Movies and TV shows, and save files directly to the specified output directory.
- `-h` or `--help`: Display the help message with usage instructions.

Sit back and let Media Batch Renamer organize and rename your media files!

## Examples

Organize files in the current directory non-recursively:

```bash
./mbr
```

Organize files in a specific directory recursively, using a custom output directory, enabling verbose mode, and without creating separate directories:

```bash
./mbr -r -v -o /path/to/output_directory -n
```

## Contributing

Contributions and suggestions are welcome! If you encounter any issues, have ideas for enhancements, or would like to contribute to the project, please feel free to open an issue or submit a pull request on this [GitHub repository](https://github.com/emilhornlund/media-batch-renamer).

## License

This script is licensed under the MIT License.

Feel free to modify and adapt the script according to your needs.
