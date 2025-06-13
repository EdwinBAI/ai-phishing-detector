# AI-Powered Phishing Email Detector (WIP)  

This project is a simple web app that spots phishing emails.  
You paste an email’s text into the page, press it and the app tells you whether it looks odd.  

What it uses:
* **Scikit-learn** – does the basic machine-learning math  
* **Streamlit** – Show the web interface  
* **Amazon Bedrock** (**planned**) – will write a short in English for each result

## Why this even exists  
I’m testing AI security ideas and hope to turn this into a real Chrome extension. Phishing still causes most breaches, so a simple tool like this can help.

**Goals**  
1. **Help people** spot bad emails right now it’s just a demo I’m testing with to see what I can make, but I’d like to turn it into a full tool with end-to-end encryption (mostly for fun).
2. **Stay fast** lightweight enough to run inside a browser tab.
3. **Leverage AWS Bedrock** for short English explanations.  

## Quick start

```bash
# make a virtual env
python -m venv .venv

# turn it on
source .venv/bin/activate        # Windows: .\.venv\Scripts\activate

# install packages
pip install -r requirements.txt

# train (or retrain) the model
python train.py

# run the app
streamlit run app.py             # then open http://localhost:8501
