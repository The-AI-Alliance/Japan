---      
layout: docs      
title: Commit File      
---      
# CommitFile

The `CommitFile` API allows you to commit a file to a GitHub repository.

## Parameters

* `repo_url`: The URL of the repository, e.g. https://github.com/The-AI-Alliance/gofannon
* `file_path`: The path of the file in the repository, e.g. example.txt
* `file_contents`: The contents of the file as a string
* `commit_message`: The commit message, e.g. 'Added example.txt'

## Example Usage

```python  
commit_file = CommitFile(api_key="your_api_key_here")  
result = commit_file.fn("https://github.com/The-AI-Alliance/gofannon", "example.txt", "Hello World!", "Added example.txt")  
print(result)  
```

This will commit a new file example.txt to the gofannon repository with the contents "Hello World!" and the commit message "Added example.txt".