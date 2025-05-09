# Contract Advisor RAG: Building A High-Precision Legal Expert LLM APP

## Introduction

This project focuses on building a high precision contract analysis tool using
Retrieval Augmented Generation (RAG). This approach leverages the power of Large
Language Models (LLMs) to retrieve relevant information from external knowledge
sources, in this case, legal contracts. The goal is to create a system that can
accurately and efficiently answer questions about contract content, acting as a
virtual legal assistant.

## Table of Contents

1. [Key Features](#key-features)
2. [Project Structure](#project-structure)
3. [Getting Started](#getting-started)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Testing](#testing)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

## Key Features

- **RAG Framework**: Leverages the LangChain framework to seamlessly integrate
  LLMs with contract data.
- **OpenAI GPT Models**: Utilizes OpenAI's GPT models for natural language
  understanding and generation.
- **AutoGen Integration**: Integration with Microsoft AutoGen to create
  conversational AI agents for a more interactive user experience.
- **Web Interface**: Provides a user-friendly web interface for users to
  interact with the system and ask questions about contract content.
- **FastAPI Backend**: Uses FastAPI to create a high-performance backend server
  for handling user requests using using websockets and allow interaction with
  the RAG pipeline.
- **Vector Database**: Employs a vector database (e.g., Chroma) to store and
  retrieve contract information efficiently.
- **Multi-Query Retrieval**: Generates multiple query variations to improve the
  chances of finding relevant information.
- **Re-ranking**: Employs re-ranking mechanisms to prioritize the most
  contextually relevant information.
- **Evaluation using RAGAS**: Includes a robust evaluation pipeline using
  metrics like accuracy, relevance, and response time to assess and improve
  performance.

## Project Structure

```
project_root/
├── .github/         # GitHub Actions workflows
├── frontend/        # React frontend code
├── backend/         # FastAPI backend code
├── src/             # Source code for RAG pipeline, utils, etc.
├── tests/           # Unit and integration tests
├── README.md        # This file
└── requirements.txt # Project dependencies
```

## Getting Started

### Prerequisites

- Python 3.9+
- pip
- Node.js v18+
- npm - for installing frontend dependencies

#### 1. Clone this repo

```
git clone git@github.com:selamt94/contract-qa-high-precision-rag.git
cd contract-qa-high-precision-rag
```

#### 2. Configure the environment

Add your OPENAI_API_KEY to a .env file in the project root directory.

## Installation

#### 1. Install dependencies

```
pip install -r requirements.txt
```

## Usage

#### 1. Start the FastAPI server

Run the command to start the FastAPI server:

```
make run-server
```

The server will start at http://localhost:8000/

#### 2. Start the React frontend

```
make run-frontend
```

On your browser access the frontend app from http://localhost:3000/

## Testing

#### 1. Run tests

To run the tests, use the following command:

```
make test
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file
for details.

