# 🧪 **LLM-Based Unit Test Generator**

*Automated unit test generation and evaluation using generative AI (GPT-4)*

## 📖 Overview

This repository provides an implementation of an **LLM-based software unit test generation tool**, developed as part of the study *“Software Unit Test Automation with LLM-Based Generative AI: Evaluating Test Quality through Code Coverage and Edge-Case Analysis”*.
It automates the generation of unit tests for Python functions using **GPT-4**, executes the generated tests, analyzes their correctness and edge-case coverage, and reports code coverage using `pytest` and `coverage.py`.

The tool offers a repeatable, efficient pipeline for test automation and is designed for integration into modern software development workflows.

---

## 🚀 Features

✅ Generates unit test files in **pytest** format using GPT-4.

✅ Covers normal and **edge-case scenarios** (e.g., division by zero, invalid inputs).

✅ Executes tests automatically and validates correctness.

✅ Measures and reports **code coverage**.

✅ Produces HTML and tabular reports.

✅ Fully automated and reproducible process.

---

## 🖼️ Demo Workflow

1️⃣ Provide Python source code with functions to be tested.

2️⃣ The tool parses the code and extracts target functions.

3️⃣ Sends each function to GPT-4 with a structured prompt.

4️⃣ Saves the generated tests in `tests/` directory.

5️⃣ Runs the tests using `pytest` and analyzes results.

6️⃣ Generates and saves code coverage reports in HTML format.

---

## 📂 Directory Structure

```
genai_test_generator/
├── math_utils.py            # Python source code with sample functions
├── tests/                    # Directory for generated test files
│   ├── test_add_llm.py
│   ├── test_divide_llm.py
│   └── test_factorial_llm.py
├── reports/                  # HTML code coverage reports
├── main.py                   # Main script to run the pipeline
├── requirements.txt          # Required Python packages
```

---

## ⚙️ Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/llm-unit-test-generator.git
cd llm-unit-test-generator
pip install -r requirements.txt
```

---

## 🧑‍💻 Usage

Run the main script:

```bash
python main.py
```

By default, it will:

* Read `math_utils.py`
* Generate tests for each function
* Run tests
* Measure coverage
* Save results

You can customize the source file or output directories by modifying `main.py`.

---

## 📊 Output

✅ Test result summary (pass/fail).

✅ Code coverage percentage.

✅ Edge-case inclusion indicators.

✅ HTML coverage report in `/reports`.

---

## 📚 Future Work

We plan to extend this tool for **more complex and large-scale codebases**, evaluating the performance of LLM-based test generation on real-world software modules and multi-function dependencies. The current pipeline will serve as a foundation for scaling up and experimenting with advanced generative AI models.

---

## 🤝 Contribution

Feel free to fork, contribute, or open issues for improvements.
If you use this tool in academic work, please cite the related paper.

---

## 📄 License

MIT License — see `LICENSE` file.

---

📬 **Contact:**
For questions or feedback:

[sevdanur.genc@balikesir.edu.tr](mailto:sevdanur.genc@balikesir.edu.tr)

[furkan.ceylan@balikesir.edu.tr](mailto:furkan.ceylan@balikesir.edu.tr)

