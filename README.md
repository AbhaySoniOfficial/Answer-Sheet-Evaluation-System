# AI Answer Sheet Grader

Hi, I'm **Abhay Soni**, a foundation level student in the **IITM BS Degree** program. This is my very first project, and I'm excited to share it!

This is a Answer Sheet Evaluation System app that runs in Google Colab. It can automatically grade a handwritten True/False quiz. You just upload a picture of the answer sheet, and it reads the answers and gives you a score.

My colab link - https://colab.research.google.com/drive/1VJ0_kjlLkmn08_FiKENMhD2XOjpJFlQB?usp=sharing

Accepts images of handwritten answer sheets in a fixed layout.
Download here –>
Sheet 1 -https://mlig-iitmbs.github.io/somsubhra-promptingtalk/assets/s1.jpeg
Sheet 2 -https://mlig-iitmbs.github.io/somsubhra-promptingtalk/assets/s2.jpeg
Sheet 3 -https://mlig-iitmbs.github.io/somsubhra-promptingtalk/assets/s3.jpeg
Sheet 4 -https://mlig-iitmbs.github.io/somsubhra-promptingtalk/assets/s4.jpeg

## How I Built This

This was a big learning experience for me. I couldn't have done it without the help of **Somsubhra Sir** and Web Administration team of Wayanad House, who guided me through the project.

Somsubra Sir - https://www.linkedin.com/in/somsubhrad/

I also used **Gemini AI** in a few specific ways to make the project better:

* **Prompt Writing:** I used it to help me write the perfect set of instructions (the "prompt") to send to the AI. This was key to making sure it could read the handwriting accurately.
* **Error Handling:** When I got stuck on bugs, I used it to help me figure out what was wrong with my code and how to fix it.

## How It Works (It's pretty simple!)

1.  **You upload an image** of the completed 10-question quiz.
2.  The app sends this picture to the Google Gemini AI to **read the handwritten** "True" or "False" answers.
3.  It then **compares those answers** to the correct answer key (which is stored in the code).
4.  Finally, it **shows you a full report** with the final score, percentage, and a letter grade.

## How to Run This in Google Colab

You can run this notebook yourself. Here's how:
You need to import the code (.ipynb) in your colab

### 1. Add Your API Key

Before you run any code, you need to add your Google AI API key.

1.  Look on the left side panel in Colab and click the **Key icon (🔑)**.
2.  Click **"Add a new secret"**.
3.  In the **Name** box, type: `GOOGLE_API_KEY`
4.  In the **Value** box, paste your real API key.
5.  Turn **ON** the "Notebook access" toggle.

### 2. Run the Cells in Order

Now, just run each code cell from the top of the notebook to the bottom.

1.  **Cell 1:** Installs all the needed libraries (`!pip install...`).
2.  **Cell 2:** Safely imports your API key from the Secrets panel.
3.  **Other Cells:** These set up all the functions (the "how-to-grade" logic).
4.  **Last Cell:** This one (with `demo.launch()`) starts the web app.

### 3. Open the App

After you run the very last cell, look at the output. Colab will show a public link that looks like this:

`Running on public URL: https://[some-random-text].gradio.live`

**Click that `.gradio.live` link!** It will open the app in a new browser tab, ready for you to upload an image.
