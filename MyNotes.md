


```python
# This is used  to hide the hard coded API key values
import os
import openai
import tiktoken
from dotenv import load_dotenv, find_dotenv
_ = load_dotenv(find_dotenv()) # read local .env file
​
openai.api_key  = os.environ['OPENAI_API_KEY']
```


- **Chain of Thought Reasoning** => Give the model time to think (for model with ~100B parameters)
- **Zero Shot Chain of Thought** => Appending the words "Let's think step by step." to the end of a question
- **Self-consistency** => Ask a model the same prompt multiple times & take the majority result as the final answer
- **Chaining Prompts** => Break down complex tasks


## Loader options

<p align="center">
  <img src ="img/loader_options.png" width = "500"   height="450" title="photo">  
</p>


## Set OPENAI_API_KEY var for win10
1. Launch “Control Panel”
2. “System”
3. “Advanced system settings”
4. Switch to “Advanced” tab
5. “Environment variables”
6. Choose “User Variable” (for just you since any other accounts on your system could access System Variables)
7.To add a new environment variable: Choose “New”
8. Enter the variable name “OPENAI_API_KEY” and the actual API string then save it.
9. You need to RE-START the Python interactive session if you have it running on your system for the new setting to take effect.
