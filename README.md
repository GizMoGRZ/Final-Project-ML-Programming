This project compares SqueezeBERT, Modified SqueezeBERT, and BERT on a text
classification task and benchmarks their inference speed using Wikipedia
sentences extracted from an XML dump.


1. Requirements
---------------------------------------------------------------------------

No local installation is needed.

All code runs entirely inside Google Colab.

The only requirement from the user is:

  Download the Wikipedia XML dump (e.g., "enwiki-20251201-pages-articles.xml-p1p41242")
  Upload the XML file into the Colab notebook session when prompted (may take a while)

Everything else is handled automatically.


2. How To Run
---------------------------------------------------------------------------

Step 1 — Open the provided Google Colab notebook.

Step 2 — Upload your Wikipedia XML file when prompted.
          The notebook will detect and process it automatically.

Step 3 — Run the notebook cells from top to bottom.
  The notebook will:
      Install all required Python libraries (Transformers, Datasets, etc.)
      Extract 1,000 clean sentences from the Wikipedia XML file
      Prepare the dataset for training
        Train:
            - SqueezeBERT Base
            - Modified SqueezeBERT
            - BERT
          Evaluate all models on accuracy and F1
          • Benchmark inference speed for all models
          • Display results for comparison

Step 4 — Review the output at the end of the notebook:
          • Training curves
          • Evaluation metrics
          • Inference speed table

No additional configuration or file editing is required.


Notes
---------------------------------------------------------------------------

No manual installation is required.
No terminal commands are needed.
All processing, extraction, training, and evaluation occur inside Colab.
The notebook automatically uses GPU if available.
