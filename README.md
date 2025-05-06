Legal documents are often complex, lengthy, and full of technical jargon. This project uses Legal BERT, a transformer-based model fine-tuned on legal text, to extract key legal entities from unstructured documents like court judgments. The goal is to transform dense legal content into structured, meaningful data that can be analyzed, visualized, or used for further processing.

Features
Named Entity Recognition (NER) for legal-specific entities using Legal BERT
Crime category classification using a BERT-based sequence classifier
Rule-based extraction for entities like court name, date, and judge
Web interface or Google Colab notebook for easy interaction
Clean and structured output format
Sample legal documents and inference examples included

Tech Stack
Model: Legal BERT (HuggingFace Transformers)

Language: Python

Libraries: Transformers, scikit-learn, pandas, NumPy, spaCy

Frontend: Streamlit / Flask (optional)

Notebook: Google Colab-compatible

Data: Curated legal judgments (academic use)

Getting Started
Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/legal-entities-extraction.git
cd legal-entities-extraction
Install Dependencies
bash
Copy code
pip install -r requirements.txt
Run on Google Colab
Open the notebook Legal_BERT_Entity_Extraction.ipynb in Google Colab.

Upload a sample legal document.

Run the cells to extract entities and classify crime types.

Run Locally (Optional Streamlit App)
bash
Copy code
streamlit run app.py
Project Structure
bash
Copy code
├── app.py                      # Streamlit app (if used)
├── Legal_BERT_Entity_Extraction.ipynb  # Colab notebook
├── models/
│   ├── legal_bert_ner/         # Fine-tuned NER model
│   └── crime_classifier/       # Crime classification model
├── data/
│   └── sample_cases/           # Sample input documents
├── utils/
│   └── extraction_rules.py     # Rule-based entity extraction
├── requirements.txt
├── README.md
Sample Output
json
Copy code
{
  "Court": "Bombay High Court",
  "Judge": "Justice A. Sharma",
  "Petitioner": "ABC Technologies Pvt. Ltd.",
  "Respondent": "XYZ Ltd.",
  "Date": "12 March 2021",
  "Crime Category": "Cyber Crime"
}
Dataset Info
Curated and anonymized legal judgment samples

Preprocessed for tokenization, entity labeling, and classification

Not publicly shared due to data sensitivity — used for academic demonstration only

Demo
Demo video or live Colab link (optional): Coming Soon

Acknowledgements
Legal BERT - NLP AUEB

HuggingFace Transformers

Various legal text corpora for academic use

Contributing
Contributions are welcome.
If you'd like to suggest changes or improve the system, feel free to fork this repository and submit a pull request.

Contact
Author: Anagha Burli
Email: codeanagha@gmail.com
GitHub: https://github.com/anaghaburli21

License
This project is licensed under the MIT License. See the LICENSE file for details.
