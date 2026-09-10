# Excluding-Machine
A machine that excludes facts and ideas from consideration.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Exclude this idea from consideration, machine." \
  | uvx excluding-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install excluding-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
excluding-machine -a multilogue.txt
```
Or:
```bash
excluding-machine multilogue.txt > response.txt
```
Or:
```bash
excluding-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import excluding_machine
```
