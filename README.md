# ✍️ LinkedIn Post Analyzer & Improver

This project features a **Google Colab** notebook designed to analyze and improve LinkedIn posts using the LLM. It leverages the power of **Python** within a Google Colab environment, interacting with the **OpenAI API** for intelligent content analysis and generation. It provides a structured critique of original posts based on key content quality metrics and generates an enhanced version, helping users craft more engaging and effective professional content.

---

## ✨ Project Objective

The primary objective of this tool is to:
* Automate the critical analysis of LinkedIn post content.
* Provide actionable feedback on various aspects of post quality and engagement.
* Generate improved versions of posts, adhering to LinkedIn best practices.
* Streamline the content creation process for professionals and marketers.

**The workflow involves :**

* **Google Drive Integration:** Securely mounts Google Drive to allow users to input their LinkedIn posts from a CSV file and save the analyzed output.
* **OpenAI API Connection:** Establishes a connection to the OpenAI API using a user's API key (stored securely in Colab Secrets).
* **Prompt Engineering:** Utilizes a carefully crafted prompt to instruct the OpenAI model (GPT-4o-mini) on how to analyze posts based on specific criteria.
* **Automated Analysis & Improvement:** Iterates through each post in the provided CSV, sends it to the OpenAI API for analysis and improvement, and parses the structured response.
* **Markdown Output & Download:** Formats the original post, AI-generated analysis, and improved version into clear Markdown, displayed directly in the notebook and compiled into a downloadable `.md` file.

---

## 🛠️ Technologies Used

* **Platform:** Google Colab
* **Programming Language:** Python
* **Libraries:**
    * `pandas` (for reading and manipulating CSV data)
    * `openai` (for interacting with the OpenAI API)
    * `google.colab` (for Google Drive integration and Colab Secrets management)
    * `IPython.display` (for rendering Markdown output within the notebook)
    * `os` (for operating system interactions, if needed for file paths)
* **API:** OpenAI (GPT-4o-mini model)

---

## 🚀 How to Use the LinkedIn Post Analyzer

This project is designed to be run interactively in Google Colab.

1.  **Open the Google Colab Notebook:**
    Click the "Open In Colab" badge below to launch the notebook directly in your browser.

   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/margarytaz/linkedin-post-analyser/blob/main/notebook/Post_Analyser.ipynb)

2.  **Set up OpenAI API Key:**
    * In Google Colab, go to the left sidebar, click the **"Secrets" (🔑) icon**.
    * Add a new secret named `OPENAI_API_KEY` and paste your OpenAI API key as its value.
    * Ensure "Notebook access" is toggled ON for this secret.

3.  **Mount Google Drive:**
    * Run the first code cell in the notebook to mount your Google Drive. This will allow the notebook to access your CSV file and save the output. Follow the prompts to authorize access.

4.  **Prepare Your CSV File:**
    * Ensure your CSV file (e.g., `my_linkedin_posts.csv`) is accessible from your Google Drive.
    * This CSV file **must** contain a column named `post_content` with the LinkedIn posts you wish to analyze.

5.  **Run the Notebook Cells:**
    * Execute all cells in the notebook sequentially.
    * When prompted, enter the full path to your CSV file on Google Drive (e.g., `/content/drive/My Drive/my_linkedin_posts.csv`).
    * When prompted, enter the desired path to save the output Markdown file (e.g., `/content/drive/My Drive/linkedin_analysis_results.md`).

6.  **Review Output:**
    * The analysis and improved versions of each post will be displayed directly in the notebook.
    * A compiled Markdown file containing all outputs will be saved to your specified Google Drive path.

---
