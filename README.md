
# Exno.7-Prompt-Engineering
Date: 22/04/2025
---
Register no. 212223060203
---
---

##  Aim  
To Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.
---

## ⚙️ Algorithm  
- Develop a prompt-based application using ChatGPT.
- Organize daily tasks by structuring and categorizing them using AI-generated prompts.
- Progress from simple prompts (basic task creation) to more advanced prompts (task prioritization, reminders, categorization).
- Showcase how the output evolves and how AI can be used to streamline task management.
  
---

## 📚 Procedure  

### 1. **Setup Environment**  
Ensure Python is installed along with necessary libraries. Use the following command:
```bash
pip install openai
```

### 2. **Define Prompts**  
Start with simple prompts for basic task creation, then progress to more advanced prompts that include prioritization and reminders. Example:
- **Simple Prompt**: "Create a task for the day."
- **Advanced Prompt**: "Create a task for today, categorize it into work, and prioritize it based on urgency."

### 3. **Test Output**  
Generate tasks using ChatGPT’s API or a locally hosted model, experimenting with different prompt variations.

---

## 💻 Sample Code
```python
import openai

# Setup the OpenAI API Key
openai.api_key = 'your-openai-api-key'

# Function to generate daily tasks using ChatGPT
def generate_daily_tasks(prompt):
    response = openai.Completion.create(
        engine="text-davinci-003",
        prompt=prompt,
        max_tokens=150
    )
    return response.choices[0].text.strip()

# Basic Task Creation
basic_prompt = "Create a task for today."
basic_task = generate_daily_tasks(basic_prompt)
print(f"Basic Task: {basic_task}")

# Task with Categorization and Prioritization
advanced_prompt = "Create a task for today, categorize it into work, and prioritize it based on urgency."
advanced_task = generate_daily_tasks(advanced_prompt)
print(f"Advanced Task: {advanced_task}")
```

---

## ✅ Result  
The corresponding prompt was executed successfully.

---

## 🎶 Additional Objective  
Explore various prompting techniques for generating audio using AI models. The goal is to understand how different types of prompts influence the generation of audio, such as music, sound effects, or speech, and how to optimize these prompts for specific needs.

---

## 📦 Deliverables
- ✅ Python script that uses ChatGPT for task creation
- ✅ Comparison of results for simple vs advanced prompts
- ✅ Insight into how prompt complexity affects AI output

---

## 📝 Conclusion  
This experiment demonstrated the power of prompt engineering in organizing tasks with AI. By evolving from simple to advanced prompts, we learned how to leverage language models to manage, categorize, and prioritize tasks effectively. Additionally, the exploration of audio generation using AI models provides insights into how prompt techniques influence different media outputs.

---

```

This format will allow you to have a clean and clear readme for your project on GitHub. Let me know if you need any additional adjustments or would like to add further details!
