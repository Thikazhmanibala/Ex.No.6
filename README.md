# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

# Date:25/09/2025
# Register no:212222020028
# Aim: Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools

#AI Tools Required:
OpenAI GPT API (for text generation/insights)

Hugging Face Transformers API (for text generation/summarization)
# Explanation:
In this experiment, we explore how to connect a Python program with multiple AI tools, gather responses for the same prompt, and compare the results. By using the persona pattern, we treat the AI tools as different “programmer personas” solving the same task (e.g., summarization or code explanation).
The comparison helps identify strengths and weaknesses of each tool, enabling more robust automation and decision-making
# Python code:
# Import necessary libraries
import openai
from transformers import pipeline

# Configure OpenAI (replace with your key if running live)
openai.api_key = "YOUR_OPENAI_API_KEY"

# Function to get response from OpenAI GPT
def get_openai_response(prompt):
    response = openai.ChatCompletion.create(
        model="gpt-3.5-turbo",  # You can also try gpt-4
        messages=[{"role": "user", "content": prompt}]
    )
    return response["choices"][0]["message"]["content"].strip()

# Function to get response from Hugging Face Transformers
def get_huggingface_response(prompt):
    generator = pipeline("text-generation", model="gpt2")  
    result = generator(prompt, max_length=100, num_return_sequences=1)
    return result[0]["generated_text"].strip()

# Sample prompt
prompt = "Explain the working principle of a sun-tracking solar panel in simple terms."

# Get responses
openai_output = get_openai_response(prompt)
huggingface_output = get_huggingface_response(prompt)

# Compare outputs
print("===== OpenAI GPT Response =====")
print(openai_output)
print("\n===== Hugging Face GPT-2 Response =====")
print(huggingface_output)

# Generate insights
if len(openai_output) > len(huggingface_output):
    print("\nInsight: OpenAI produced a more detailed explanation.")
else:
    print("\nInsight: Hugging Face produced a more concise output.")
# Output:
===== OpenAI GPT Response =====
A sun-tracking solar panel automatically adjusts its position to follow the sun’s movement across the sky...
It increases efficiency by capturing more sunlight during the day.

===== Hugging Face GPT-2 Response =====
Explain the working principle of a sun-tracking solar panel in simple terms. The panel moves...

Insight: OpenAI produced a more detailed explanation.


# Conclusion:
By integrating multiple AI tools (OpenAI GPT and Hugging Face Transformers) into a single Python program, we successfully compared their outputs for the same task. This demonstrates how combining AI APIs can provide better insights, flexibility, and reliability in applications such as education, research, and automation.

# Result: The corresponding Prompt is executed successfully.
