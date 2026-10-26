# Verb-Machine
A machine executing an action defined by the verb.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Think about it, machine!" \
  | uvx verb-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install verb-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
verb-machine -a multilogue.txt
```
Or:
```bash
verb-machine multilogue.txt > response.txt
```
Or:
```bash
verb-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import verb_machine
```
