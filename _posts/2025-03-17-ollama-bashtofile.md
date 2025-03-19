---
layout: post
title:  "Using Ollama CLI to Prompt and Write to Files"
date:   2025-03-17 12:07:21 -0500
---
The **Ollama CLI** allows you to run AI models directly from the terminal, making it easy to generate text and save it to files for later use. This is particularly useful for automating AI-generated content, summaries, or responses.

In this guide, we’ll walk through:  
1. How to prompt Ollama and write its output to a file.  
2. A **Bash script example** to automate this task.

---

## **1. Running Ollama and Saving Output to a File**  

To prompt **Ollama** and save its response to a file, you can use the following command:  

```bash
ollama run <model_name> "Your prompt here" > output.txt
```

For example, if you want to generate a short story using **GPT-3.5**, run:

```bash
ollama run gpt-3.5 "Write a short science fiction story." > story.txt
```

This will:  
- Send the prompt `"Write a short science fiction story."` to the Ollama model.  
- Save the response in **story.txt** instead of displaying it in the terminal.  

💡 **Tip:** If you want to append output instead of overwriting the file, use `>>` instead of `>`:  

```bash
ollama run gpt-3.5 "Continue the story." >> story.txt
```

---

## **2. Using a Bash Script to Automate the Process**  

Let’s create a **Bash script** that:  
✅ Takes a prompt as input.  
✅ Runs the prompt through Ollama.  
✅ Saves the AI-generated text to a file.  

### **Bash Script Example: `ollama_writer.sh`**  

```bash
#!/bin/bash

# Check if a prompt was provided
if [ -z "$1" ]; then
  echo "Usage: $0 'Your prompt here'"
  exit 1
fi

# Define the model and output file
MODEL="gpt-3.5"
OUTPUT_FILE="ollama_output.txt"

# Run Ollama and save output to file
ollama run "$MODEL" "$1" >> "$OUTPUT_FILE"

# Notify the user
echo "Response saved to $OUTPUT_FILE"
```

---

## **3. How to Use the Bash Script**  

### **Step 1: Make the Script Executable**  
First, give your script execute permissions:  

```bash
chmod +x ollama_writer.sh
```

### **Step 2: Run the Script with a Prompt**  

Use the script by providing a prompt as an argument:  

```bash
./ollama_writer.sh "Write a motivational quote."
```

This will generate a **motivational quote** using the **GPT-3.5 model** and save it in `ollama_output.txt`.

---

## **4. Advanced: Automating Multiple Prompts**  

To process multiple prompts from a text file (`prompts.txt`), use:  

```bash
while read prompt; do
  ./ollama_writer.sh "$prompt"
done < prompts.txt
```

This will loop through each line in `prompts.txt`, run it through Ollama, and save all responses in `ollama_output.txt`.

---

## **Conclusion**  

The **Ollama CLI** is a powerful tool for AI-powered content generation. By using a **Bash script**, you can automate tasks like writing articles, generating ideas, or summarizing text—all from the command line.

Try it out and let me know what creative uses you come up with! 🚀

Additional Reading:
- [Running Ollama Via Terminal](https://www.hostinger.com/tutorials/ollama-cli-tutorial?utm_medium=ppc&utm_campaign=Generic-Tutorials-DSA|NT:Se|LO:CA&gad_source=1#Prompting_and_logging_responses_to_files)
