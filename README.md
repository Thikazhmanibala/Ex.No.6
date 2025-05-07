# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

### Date: 07-05-2025
### Deevloped by: RAMYA R
### Register no: 212223230169
# Aim:
Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools


## 🎯 Objective
To write and implement Python code that interacts with multiple AI tools (such as OpenAI's ChatGPT, Anthropic's Claude, Google Gemini, and Microsoft Copilot) using their respective APIs. The goal is to automate:
- Submitting a common prompt
- Comparing the returned outputs
- Generating actionable insights based on defined evaluation metrics (e.g., accuracy, coherence, simplicity)

---

## ⚙️ Use Case
**Healthcare Diagnostics**: The system will automate the analysis of patient symptoms and generate diagnostic insights by interacting with multiple AI platforms, enabling healthcare professionals to make informed decisions more efficiently.

---

# 🔍 AI Tools Required:

## CHATGPT
## CLAUDE
## GEMINI

## 📌 Algorithm Overview

### **Step-by-Step Algorithm for Multi-AI Tool Integration**

1. **Set Up API Integrations**:
   - Install necessary libraries and set up the credentials for each AI tool: **ChatGPT**, **Claude**, and **Gemini**.
   - Use `requests` or other relevant libraries for API integration.

2. **Input Healthcare Query**:
   - Accept healthcare-related data such as symptoms, medical history, and test results.

3. **Format Prompts**:
   - Three types of prompts will be used:
     - **Straightforward Prompt**: Asking for a diagnosis based on patient symptoms.
     - **Tabular Format**: Presenting data in a table format for structured input.
     - **Missing Word Prompt**: Providing a partially completed sentence for prediction.
   
4. **Submit Prompts to Each AI Tool**:
   - Send the formatted prompts to **ChatGPT**, **Claude**, and **Gemini** APIs.

5. **Receive and Parse Responses**:
   - Collect and extract useful information such as diagnosis and treatment suggestions.

6. **Comparison of Outputs**:
   - Compare the responses based on **accuracy**, **clarity**, **simplicity**, and **user experience**.

7. **Generate Actionable Insights**:
   - Provide a summary of findings and suggest which tool performs best for specific types of queries.

8. **Create Final Report**:
   - Compile the results and insights into a comprehensive evaluation report.

---

## 🧪 Prompt Types

- **Straightforward Prompt**: A simple query asking for diagnosis and treatment based on provided symptoms.
  
- **Tabular Format**: Presenting data in a structured table format for each symptom.
  
- **Missing Word Prompt**: A prompt with an incomplete sentence for the AI to complete.

## 📤 Example Queries & Responses

### 1. **Straightforward Prompt**
**Prompt:**  
"Patient reports fever, cough, and shortness of breath. What could be the diagnosis and recommended action?"

| **AI Tool**   | **Response**                                                       |
|---------------|--------------------------------------------------------------------|
| **ChatGPT**   | Likely pneumonia. Recommend chest X-ray, antibiotics, and rest.   |
| **Claude**    | Possibly COVID-19 or pneumonia. Suggests COVID test, X-ray, and oxygen monitoring. |
| **Gemini**    | Likely pneumonia, suggest X-ray, and antibiotics, recommend further blood tests for confirmation. |


### 2. **Tabular Format Prompt**
**Prompt:**

| **Symptom** |	**Present** |
|-------------|-------------|
| **Fever**   |	**Yes**     |
| **Cough**   |	**Yes**     |
| **Chest Pain** |	No      |
| **Difficulty Breathing** |	**Yes**     |

# Explanation:
Experiment the persona pattern as a programmer for any specific applications related with your interesting area. 
Generate the outoput using more than one AI tool and based on the code generation analyse and discussing that. 

# Conclusion:


# Result: The corresponding Prompt is executed successfully.
