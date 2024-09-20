# MaskitLLM – Advanced LLM Sensitive Information Masking Service

## Overview

**MaskitLLM** is a state-of-the-art sensitive information masking service designed to protect private data before transmission to Large Language Models (LLMs) such as GPT. This service leverages cutting-edge NLP techniques to automatically identify and mask critical information, providing a robust solution for data privacy in AI-driven environments. The initial prototype is implemented using **Streamlit** for rapid iteration and user feedback, while the production version will be built with **FastAPI** for scalability and performance.

## Key Features

- **Intelligent Sensitive Data Masking**: Utilizes advanced NLP models to detect and mask a wide range of sensitive information including but not limited to personal identifiers, financial data, and proprietary information.
- **Interactive Text Comparison**: Provides a side-by-side view of original and masked text with highlighting for easy verification.
- **Customizable Masking Rules**: Allows users to define custom masking rules and sensitivity levels tailored to specific use cases or industries.
- **Manual Refinement**: Enables fine-grained control through manual selection and masking of text segments.
- **Secure Export Options**: Offers various secure export formats for seamless integration with LLM pipelines.
- **API Integration**: (Planned) RESTful API for easy integration into existing workflows and applications.

## Technology Stack

- **Python 3.9+**: Leveraging the latest language features for robust and efficient code.
- **Streamlit**: For rapid prototyping and interactive testing interface.
- **FastAPI**: High-performance framework for production API deployment.
- **SpaCy**: State-of-the-art NLP library for Named Entity Recognition (NER) and linguistic analysis.
- **Hugging Face Transformers**: Cutting-edge pre-trained models for advanced NLP tasks.
- **PostgreSQL**: (Planned) For storing user preferences and masking rules.
- **Docker**: For containerization and easy deployment.

## Installation and Setup

### Prerequisites

- Python 3.9+
- Docker (optional, but recommended for production deployment)
- Git

### Development Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/kunwookim/maskitllm.git
   cd maskitllm
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Install pre-commit hooks for code quality:
   ```bash
   pre-commit install
   ```

### Running the Service

#### Development (Streamlit):

```bash
streamlit run src/streamlit_app.py
```

#### Production (FastAPI):

```bash
uvicorn src.main:app --host 0.0.0.0 --port 8000 --workers 4
```

For containerized deployment:

```bash
docker-compose up --build
```

## Project Roadmap

### Phase 1: Prototype and Data Collection (Current)

- Implement core masking functionality using Streamlit
- Collect user feedback and real-world data for model improvement

### Phase 2: Advanced NLP Integration

- Incorporate fine-tuned transformer models for improved entity recognition
- Implement context-aware masking to reduce false positives

### Phase 3: Production API Development

- Develop FastAPI backend with rigorous security measures
- Implement user authentication and role-based access control

### Phase 4: Scalability and Performance Optimization

- Optimize for high-throughput processing
- Implement caching and database integration for improved performance

### Phase 5: Enterprise Features

- Develop customizable dashboards for analytics and audit trails
- Implement advanced encryption for masked data storage

## Contributing

We welcome contributions from the community. Please refer to our [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines on how to contribute effectively to this project.

## Security

Security is our top priority. If you discover any security-related issues, please email security@maskitllm.com instead of using the issue tracker.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

We would like to thank the open-source community and the creators of the libraries and tools that make this project possible. Special thanks to our early adopters and contributors for their valuable feedback and support.
