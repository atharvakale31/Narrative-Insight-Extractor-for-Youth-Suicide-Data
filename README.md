
# Narrative Insight Extractor for Youth Suicide Data

This project provides an **automated data abstraction tool** designed to extract standardized variables from law enforcement narratives on youth suicide cases. Built using an LLM (Large Language Model), the tool translates unstructured text data into structured insights, enabling researchers and analysts to quickly access key variables from narrative accounts. This project focuses on making the data extraction process for binary and categorical variables streamlined, accurate, and efficient.

## Features

- **Automated Narrative Parsing**: Leverages a fine-tuned model to extract binary and categorical variables from law enforcement and medical examiner narratives in youth suicide cases.
- **Flexible Prompting System**: The model uses carefully structured prompts to understand and categorize variables based on specific categories such as **InjuryLocationType** and **WeaponType1**.
- **Batch Processing**: Processes large datasets by batching inputs, ideal for handling extensive narrative records.
- **Robust Error Handling**: Includes parsing functions to manage errors or unrecognized outputs and logs warnings for easy debugging.
- **Deployment-ready**: Designed to be deployed on platforms like Streamlit for an interactive user experience.

## How It Works

1. **Data Processing**: Takes narrative text inputs and preprocesses them to align with model expectations.
2. **Model Prompting**: Uses structured prompts to guide the model in extracting relevant variables.
3. **Output Parsing**: Converts model outputs into JSON format, then maps them into a standardized CSV format for submission.
4. **Interactive Analysis**: The tool is deployable as an interactive app, allowing users to input narratives directly and receive standardized outputs.

## Getting Started


1. **Download Model**: Run `save_model()` to download and configure the necessary model files.
2. **Input Narratives**: Place narrative data in the specified format, or use the example data provided.
3. **Run Predictions**: Use `predict_on_batch()` to generate predictions for batches of narratives.
4. **Parse Outputs**: Run the output parsing functions to transform model responses into submission-ready format.


## Future Improvements

- **Model Optimization**: Experiment with different configurations and prompts to improve extraction accuracy.
- **Deployment**: Deploy on a platform like Streamlit or Hugging Face Spaces for public access.
- **Enhanced Error Handling**: Expand parsing logic to address more edge cases in narrative data.



