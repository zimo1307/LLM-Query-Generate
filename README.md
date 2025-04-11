
# 📊 LLM-Powered SQL Query System

This project allows users to ask questions about employee activity data in natural language. The system uses a large language model (LLM) to generate SQL queries and summarize the results. It also supports data visualization and provides an interactive query interface with Gradio.

---

## ✅ Step 1: Set Your OpenAI API Key

Find the code block below and replace `"your_openai_api_key"` with your actual OpenAI API key.

```python
client = OpenAI(api_key="your_openai_api_key")
```

You can find this part in the first cell of the notebook (as shown in the first screenshot).

---

## ✅ Step 2: Initialize Database and Load API Functions

Before using the system, you must first:

1. Run the **data generation and database initialization cell** (shown in the second screenshot).
2. Then run the **OpenAI API interaction function cell**, which sets up the function `ask_llm()`.

Make sure both of these are executed before moving forward.

---

## ✅ Step 3: Benchmark 2: Re-testing After Improvements

To quickly test the main functionality, run the code section under:

```
Benchmark 2: Re-testing After Improvements
```

This will automatically run 20 benchmark queries using the improved prompt and system design. It will generate summaries using the LLM and show how the system behaves in its final version.

---

## ✅ Step 4: Data Visualization

If you want to explore chart generation:

1. Run the `Data Visualization` section.
2. The system will automatically choose between **line chart**, **bar chart**, or **pie chart** based on SQL result structure.
3. Output images will be saved as `output_plot.png`.

---

## ✅ Step 5: Gradio Interface (Optional)

To test the full interactive experience:

1. Make sure you have already run the `Data Visualization` code (as the visualization code is reused).
2. Then run the final section with the Gradio interface (shown in the last screenshot).

This will launch a small web interface that lets you input natural language queries and view responses and charts.

---

## ⚠️ Notes

- Do **not** upload your real OpenAI API key to public GitHub repositories.
- My API key has reached its usage limit, so some screenshots of results were taken via phone.
- You are free to use the code and adjust the prompts, visual logic, or database structure.
