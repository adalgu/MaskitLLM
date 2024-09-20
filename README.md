# MaskitLLM – Advanced Sensitive Information Masking for LLMs

![image](https://github.com/user-attachments/assets/2e8e514c-dacb-4848-8446-a8841533c3d9)

## Overview

**MaskitLLM** is a sophisticated service designed to ensure the protection of sensitive information before it's transmitted to Large Language Models (LLMs) such as GPT. The service employs advanced Natural Language Processing (NLP) techniques to automatically detect and mask sensitive data, providing a robust solution for data privacy in AI-driven workflows.

**MaskitLLM** integrates seamlessly with modern frameworks such as **Langchain**, enabling automated pre-processing of sensitive data before it enters any LLM pipeline. The upcoming feature allowing data restoration through secure authentication further enhances the service, providing users with complete control over their data at every step.

## Key Features

- **Automated Sensitive Data Masking**: Detects and masks personal identifiers, financial data, proprietary information, and more using advanced NLP models.
- **Langchain Integration**: (Upcoming) Effortless integration with Langchain, enabling real-time sensitive data masking within LLM workflows.
- **Secure Data Restoration**: (Future) A passcode-protected mechanism that restores masked data to its original form, giving users full access to LLM-generated outputs while maintaining data security throughout the process.
- **Interactive Comparison Tool**: View original and masked text side by side, with intuitive highlights for easy verification.
- **Customizable Masking Rules**: Tailor masking rules to meet specific needs across industries, ensuring flexibility and precision in data handling.
- **Manual Refinement**: Provides users with granular control over masking, allowing manual adjustments to meet exact requirements.
- **API for Seamless Integration**: (Planned) A RESTful API for easy incorporation into existing enterprise applications and workflows.
- **Enterprise-Grade Security and Scalability**: Designed for scalability, with strong encryption protocols and secure export options for data privacy at scale.

## Technology Stack

- **Python 3.9+**: Core language for performance and flexibility.
- **Streamlit**: Enables rapid prototyping and interactive testing interfaces.
- **FastAPI**: High-performance, production-ready API framework.
- **SpaCy**: Advanced NLP library for Named Entity Recognition (NER) and linguistic analysis.
- **Hugging Face Transformers**: Pre-trained models for accurate recognition of sensitive data.
- **PostgreSQL**: (Planned) Database integration for storing user preferences and custom rules.
- **Docker**: Ensures streamlined deployment in various environments.

## Installation and Setup

### Prerequisites

- Python 3.9+
- Docker (optional, recommended for production)
- Git

### Quick Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/adalgu/maskitllm.git
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

#### Development Mode (Streamlit):

```bash
streamlit run src/streamlit_app.py
```

#### Production Mode (FastAPI):

```bash
uvicorn src.main:app --host 0.0.0.0 --port 8000 --workers 4
```

For containerized deployment:

```bash
docker-compose up --build
```

## Project Roadmap

![image](https://github.com/user-attachments/assets/e3fb24e0-9790-4d43-8818-7db1e8e21529)

### Phase 1: Functional Prototype (Current)

- Core masking features implemented and deployed.
- Collecting user feedback to refine NLP models and performance.

### Phase 2: Langchain Integration (Upcoming)

- Seamless integration with Langchain for real-time sensitive data masking.
- Automated pre-processing for improved efficiency and security in LLM workflows.

### Phase 3: Advanced NLP Customization

- Enhanced NLP models for improved recognition accuracy and reduced false positives.
- Customizable industry-specific rules for sensitive data masking.

### Phase 4: Data Restoration via Secure Authentication

- Development of a secure passcode-protected restoration process for masked data.
- Enables users to safely handle raw data after LLM processing, unlocking full utility while maintaining privacy.

### Phase 5: Enterprise-Grade API

- FastAPI backend development, with advanced encryption and role-based access control.
- Secure API for large-scale deployment.

### Phase 6: Scalability and Enterprise Features

- Optimized for high-performance, scalable operations.
- Advanced analytics dashboards and audit trails for enterprise compliance.

## Contributing

We welcome contributions from the community. Please refer to our [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines on how to get involved.

## Security

Data security is at the forefront of our development process. If you identify any security issues, please report them to ensure rapid resolution.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

A big thank you to the open-source community and our early adopters for their invaluable feedback and contributions. Your support continues to drive MaskitLLM forward.
