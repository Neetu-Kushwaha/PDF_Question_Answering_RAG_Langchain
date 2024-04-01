# Semi-Structured RAG Langchain

This project is designed to process semi-structured documents and perform question answering using the Retrieval-Augmented Generation (RAG) techniques with the Langchain library.

## Installation

1. Install the required dependencies listed in the `requirements.txt` file:

    ```bash
    pip install -r requirements.txt
    ```

2. ### Command Line Arguments

   When running the scripts, you can specify command line arguments to customize the behavior:

   - `--filename`: Path to the PDF file to be processed. Default is `./data/attention.pdf`.
   - `--path`: Path to the directory containing the PDF file. Default is `/Users/nkushwaha/PycharmProjects/semi_structured/Semi_structured_RAG_Langchain/`.



## Usage

### PDF Processing

Use the provided `pdf_processor.py` script to parse PDF documents and extract text and tables.

### Element Class

The `element.py` script contains the `Element` class, which is a Pydantic model used to represent elements extracted from PDFs.

### Text Processing

Basic text processing functions are provided in the `text_processing.py` script.

### Summarization

Summarization of text and tables can be performed using the `summarization.py` script.

### Question Generation

Question answering can be performed using the `generation.py` script, which generates responses based on prompts and embeddings.

### Embedding

Text embeddings can be generated using the `embedding.py` script.

### Main Script

The `main.py` script orchestrates the entire process, from reading PDF files to generating answers to user questions.

### Running the Main Script

To run the main script, use the following command:

```bash
python main.py --filename <path_to_pdf_file> --path <directory_containing_pdf_file>
```
### Note

Make sure to set up your OpenAI API key in your environment or directly in the script if you plan to use OpenAI services.

### Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

### License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
