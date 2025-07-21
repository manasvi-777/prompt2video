# 🎬 Manim + Groq: LLM-Generated Math Animations

This project uses the **Groq API (LLaMA 3.3 model)** to automatically generate **Manim animation code** from **natural language prompts**, which is then executed and rendered directly inside a notebook.

Perfect for educators, researchers, and developers who want to transform **math/geometry descriptions** into **animations** with minimal effort.

---

## 📌 Demo

 **Live on Google Colab:** [Click here to open the notebook](https://colab.research.google.com/drive/1ugcOcntrRqDp2CyIctr0MYndGSbLE-mR#scrollTo=K6CA1w5nce_G)

### How to Run the Demo Successfully

1.  **Set Your API Key**

    Add your Groq API key using:

    ```python
    import os
    os.environ["GROQ_API_KEY"] = "your_groq_key_here"
    ```

2.  **Enter a Clear Prompt**

    Example prompt:
    `"Draw a red circle, scale it to twice its size, and move it right."`

3.  **Check Output**

    * The LLM generates Python code.
    * The code is saved and run with Manim.
    * A video is rendered and displayed in the notebook.

---

## 🧠 How It Works

* You input a natural language prompt.
* Groq's LLaMA 3.3-70B model generates a valid Manim scene.
* The code is saved to `generated_manim_scene.py`.
* Manim renders the scene and creates a video.
* The output video is shown in the notebook or can be downloaded.

---

## 📁 Project Structure

* **generated_manim_scene.py** # Auto-generated Manim code
* **media/** # Rendered videos and images by Manim
* **Prompt2Video.ipynb** # Main Colab notebook
* **README.md** # Documentation
---
## 🚀 Future Improvements

* Deploy as a REST API using FastAPI or Flask
* Add a Gradio or Streamlit frontend
* Add safety and syntax checks for generated code
* Improve prompt templates for accuracy
* Add download/share buttons for rendered videos
