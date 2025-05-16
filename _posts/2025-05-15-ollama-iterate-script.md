---
layout: post
title:  "Automating Documentation Generation with Bash and Ollama"
date:   2025-05-15 12:07:21 -0500
---
Absolutely! Here’s a draft article that explains your Bash automation workflow, tailored for readers interested in scripting, AI, and productivity.

---

When you have a collection of source files that need documentation, manually processing each file can be tedious and time-consuming. By leveraging Bash scripting and the Ollama large language model, you can automate this workflow and generate consistent documentation for every file in your project.

### Why Automate Documentation?

- **Efficiency:** Save hours by processing files in bulk.
- **Consistency:** Use the same prompt for all files, ensuring uniform documentation style.
- **Scalability:** Easily apply the workflow to large codebases or text collections.

---

## Part 1: Generating Documentation with Ollama

The first script iterates over every file in a `source` directory, sends each file’s content to Ollama with a generic prompt, and saves the AI-generated documentation to an output folder.

```bash
#!/bin/bash

# Set your main prompt here
main_prompt="Write documentation for this content: "

# Function to remove ANSI color codes from output
remove_ansi_codes() {
    perl -CSD -pe 's/\e\[?.*?[\@-~]//g'
}

for file in source/*; do
    text_content=$( output/main/$filename"

    echo "Executing docker command for main output on: $file"
    eval "$commandbase"
done

# Clean up the output files by removing any ANSI codes and leading non-letter characters
find output/ -type f | while read -r file; do
    echo "Processing: $file"
    file_content=$(remove_ansi_codes  "$file"
    else
        echo "$file_content" > "$file"
    fi
done

echo "Build complete!"
```

**How it works:**
- Reads each file in the `source` directory.
- Combines the file content with a customizable prompt.
- Sends the combined text to Ollama via Docker.
- Writes the AI-generated documentation to `output/main/` with the same filename.
- Cleans the output by removing any unwanted ANSI color codes and extraneous characters.

---

## Part 2: Standardizing Quotes in Source Files

Before generating documentation, you might want to standardize the formatting of your source files. For example, you can replace all double quotes with single quotes using this simple Bash script:

```bash
#!/bin/bash

folder_path="source"

# Loop through all files in the folder
for file in "$folder_path"/*; do
  # Use sed to replace double quotes with single quotes in-place
  sed -i "s/\"/'/g" "$file"
done

echo "All double quotes have been replaced with single quotes in the 'source' folder."
```

**How it works:**
- Iterates over all files in the `source` directory.
- Uses `sed` to perform an in-place replacement of double quotes with single quotes.

---

## Putting It All Together

1. **Preprocess your files** (if needed) with the quote-replacement script.
2. **Run the documentation generation script** to automate the creation of documentation for each file.
3. **Review the output** in the `output/main` directory.

This approach saves you from repetitive manual work, ensures consistency, and lets you harness the power of AI for documentation at scale.

---

### Tips for Customization

- **Change the prompt:** Edit the `main_prompt` variable to suit your project’s needs.
- **Switch models:** Adjust the Ollama model in the Docker command if you want to use a different LLM.
- **Integrate other preprocessing steps:** Add more Bash or Python scripts to further clean or analyze your source files before documentation.


