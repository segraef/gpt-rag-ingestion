<!-- 
page_type: sample
languages:
- azdeveloper
- powershell
- bicep
products:
- azure
- azure-ai-foundry
- azure-openai
- azure-ai-search
urlFragment: GPT-RAG
name: Multi-repo ChatGPT and Enterprise data with Azure OpenAI and AI Search
description: GPT-RAG core is a Retrieval-Augmented Generation pattern running in Azure, using Azure AI Search for retrieval and Azure OpenAI large language models to power ChatGPT-style and Q&A experiences.
-->
# GPT-RAG Data Ingestion

Part of the [GPT-RAG](https://github.com/Azure/gpt-rag) solution.

The **GPT-RAG Data Ingestion** service automates the processing of diverse document types—such as PDFs, images, spreadsheets, transcripts, and SharePoint files—preparing them for indexing in Azure AI Search. It uses intelligent chunking strategies tailored to each format, generates text and image embeddings, and enables rich, multimodal retrieval experies for agent-based RAG applications.

### How the Data Ingestion Works

_This section will be updated soon to include a detailed explanation of the data ingestion flow, chunking strategies and connectors._

## Prerequisites

Before deploying the web application, you must provision the infrastructure as described in the [GPT-RAG](https://github.com/azure/gpt-rag/tree/feature/vnext-architecture) repo. This includes creating all necessary Azure resources required to support the application runtime.


## How to deploy the data ingestion service

Clone this repository and then run:
```shell
azd env refresh
azd deploy 
```

> [!IMPORTANT]
> When running `azd env refresh`, make sure to use the **same subscription**, **resource group**, and **environment name** that you used during the infrastructure deployment. This ensures consistency across components.

## Release 1.0.0

> [!NOTE]
> If you want to use GPT-RAG original version, simply use the v1.0.0 release from the GitHub repository.

## 🤝 Contributing

We appreciate contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on the Contributor License Agreement (CLA), code of conduct, and submitting pull requests.

## Trademarks

This project may contain trademarks or logos. Authorized use of Microsoft trademarks or logos must follow [Microsoft’s Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general). Modified versions must not imply sponsorship or cause confusion. Third-party trademarks are subject to their own policies.