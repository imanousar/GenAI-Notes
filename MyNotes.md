


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


- **Chain of Thought Reasoning** => Give the model time to think
