# Asalam alaikum warahmatullah wabarakatu!

I'm Mustafa Shoukat, a Generative AI Expert. I'm in the world of LLMs and exploring various concepts and techniques to enhance my skills. In this repository, I'll unlock the potential of Google PaLM for code generation with precision and efficiency.

_"Community empowers growth through shared knowledge and mutual support."_

Dive into code generation using Google PaLM and LangChain in this notebook. 💻🔧 Explore automated code generation, including functions, data loading, and Hugging Face models. 🤖📊✨ Get hands-on with practical examples and see the power of these tools in action! 📈📝🔍🌟💬💡

[Code Gen App | Google PaLM & LangChain 🚀💻](https://www.kaggle.com/code/mustafashoukat/code-gen-app-google-palm-langchain/edit)

## Contact Information

| Name           | Email                          | LinkedIn                                                        | GitHub                                              | Kaggle                                               | LeetCode                                                 |
|----------------|--------------------------------|-----------------------------------------------------------------|-----------------------------------------------------|-----------------------------------------------------|----------------------------------------------------------|
| Mustafa Shoukat | mustafashoukat.ai@gmail.com    | [LinkedIn Badge](https://www.linkedin.com/in/mustafashoukat/)   | [GitHub Badge](https://github.com/Mustafa-Shoukat1) | [Kaggle Badge](https://www.kaggle.com/mustafashoukat) | [LeetCode Badge](https://leetcode.com/u/MustafaShoukat/) |

![Sample Image](https://i.ytimg.com/vi/R6WNU28MgQ0/maxresdefault.jpg)

## Installing Libraries

```bash
!pip install langchain google-api-python-client
```

## Integrating Google PaLM LLM with LangChain using API

```python
from langchain.llms import GooglePalm

api_key = 'AIzaSyCWtLDiKOfa_5_GNV-4cNTjD0Z6To1gt40'
llm = GooglePalm(google_api_key=api_key, temperature=0.2)
```

## Make Test Predictions via Google PaLM

```python
llm("What is Generative AI and the role of Google PaLM? Tell me in one line.")
```

## Define a Prompt Template for Code Generation

```python
from langchain.prompts import PromptTemplate

# Define a prompt template for code generation
prompt_template = PromptTemplate(
    input_variables=["task"],
    template="Generate a {task} in Python.",
)
prompt_template
```

## Define a Function for Code Generation

```python
def generate_code(task):
    prompt = prompt_template.format(task=task)
    return llm.invoke(prompt)
```

## User Queries for Code Generation

```python
tasks = [
    "Function that calculates the factorial of a number",
    "Function to find the maximum element in an array",
    "Give me code for a complete application of langchain.llms with Google PaLM code generation application",
    "Give me code to load SQL with Python in a Jupyter notebook",
    "Give me code to load NLP reviews classification model for Hugging Face"
]
```

## Generate Code for Each Task

```python
for task in tasks:
    print(f"Task: {task}\n")
    print(f"Generated Code:\n{generate_code(task)}\n")
    print("="*50 + "\n")
```

## Define Complex Query for Code Generation

```python
print(f"Generated Code:\n{generate_code('''Create dummy data and generate code to load a sentiment analysis model from the Hugging Face pipeline using a simple model. Provide the complete code for a Kaggle kernel.''')}\n")
print("="*50 + "\n")
```

## Additional Information

<h1 style="color: #6a0dad; font-family: 'Times New Roman', Times, serif;">Integrating Google PaLM LLM with LangChain using API</h1>

![Sample Image](https://th.bing.com/th/id/OIP.HMwi10r0TW11pUc-9yZEeQHaE8?rs=1&pid=ImgDetMain)
