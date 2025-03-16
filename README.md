# GitHub Upload Script

This script uploads files to a GitHub repository using the GitHub API.

## Requirements

- Python 3.x
- Git

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/yourrepository.git
    cd yourrepository
    ```

2. Set the `GITHUB_UPLOAD_API_TOKEN` environment variable with your GitHub personal access token:
    ```sh
    export GITHUB_UPLOAD_API_TOKEN=your_token_here
    ```

## Usage

To upload files to your GitHub repository, run the script with the following command:
```sh
ghupload [-h] [--message MESSAGE] [--branch BRANCH] [files ...]
```

```
positional arguments:
  files

options:
  -h, --help            show this help message and exit
  --message, -m MESSAGE
  --branch, -b BRANCH
```

## Example
```sh
ghupload --message "Add new files" --branch "main" example.txt
```

## Notes
* Ensure that your GitHub personal access token has the necessary permissions to upload files to the repository.
* Do not hardcode your token in the script or any files that might be pushed to the repository.