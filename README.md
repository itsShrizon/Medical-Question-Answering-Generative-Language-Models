
# Enhancing Medical Question Answering with Retrieval Augmentation and Reranking Transformer Embeddings in Generative Language Models

## Authors
- Tanzir Hossain (20301154), BRAC University, Bangladesh  
- Shabab Abdullah (20301005), BRAC University, Bangladesh  
- Ar-Rafi Islam (20301164), BRAC University, Bangladesh  
- Jannatul Ferdoshi (20301193), BRAC University, Bangladesh  
- Annajiat Alim Rasel, BRAC University, Bangladesh  

## Abstract
This research presents a specialized Retrieval Augmented Generation (RAG) model designed for healthcare applications. The model combines large-scale language models with advanced retrieval approaches, utilizing Facebook AI Similarity Search (FAISS) vector store for efficient medical database searches. Key features include the "intfloat/e5-large-v2" embedding model and "RecursiveCharacterTextSplitter" for improved context alignment. The system employs mixed precision training and 4-bit neural float quantization for optimized performance.

## 1. Introduction
The integration of artificial intelligence with healthcare has shown significant potential for advancing medical research, diagnosis, and therapy. The study focuses on creating a RAG system that combines state-of-the-art language models with sophisticated retrieval techniques to enable efficient access to medical information.

## 2. Background
The emergence of large language models and advanced retrieval methods has created new opportunities for improving medical question answering systems. RAG models demonstrate proficiency in quickly navigating extensive medical databases using compact retrieval techniques powered by FAISS vector storage.

## 3. Method

### 3.1 Design
The RAG model design combines large language models with high-performance retrieval techniques for medical query and text generation.

### 3.2 Retriever Component Architectures
- **Vector Database Storage**: Utilizes FAISS for efficient similarity searching and clustering.
- **Text Chunking and Embedding**: Implements 'intfloat/e5-large-v2' embedding model with RecursiveCharacterTextSplitter.

### 3.3 Generator Component Architectures
- Uses `mistralai/Mistral-7B-Instruct-v0.1` model optimized for medical datasets.
- Implements 4-bit neural float quantization.
- Employs mixed precision training for enhanced performance.

### 3.4 Objectives
- Develop a state-of-the-art RAG model for medical query tasks.
- Provide healthcare professionals with reliable medical knowledge access.
- Build a robust information retrieval system for medical datasets.

### 3.5 Study Selection
Data source: **Medeasy** website ([www.medeasy.com](http://www.medeasy.com))  
- Comprehensive medical information collection.  
- Trusted reputation in healthcare community.  
- Regular updates by medical professionals.  
- User-friendly interface.

## 4. Results

### 4.1 Data Space

-Dataset is scraped from Meadeasy, using selenium 
- Initial dataset: 4,831 rows, 7 columns. 
- Processed dataset: 4,627 rows after cleaning.  
- Cleaning process included:
  - HTML tag removal.  
  - URL removal.  
  - Stop word removal.  
  - Irrelevant pattern removal.

### 4.2 Visual Space
Detailed visualization of data transformation and cleaning processes.

### 4.3 Interaction Space
Text-based interface for medical queries with contextualized responses.

### 4.4 Chatbot Output
Successfully demonstrated capabilities in:
- Providing medical information.  
- Identifying treatment options.  
- Offering medication suggestions with appropriate disclaimers.  
- Maintaining ethical guidelines in medical advice.

## 5. Discussion

### 5.1 V3CTRON Data Retrieval System
- Enhanced document accessibility.  
- Context-aware search capabilities.  
- Integration with various vector databases.

### 5.2 RankVicuna
- Zero-shot listwise document reranking.  
- Open-source approach to reranking tasks.  
- Comparable performance to GPT-3.5.

### 5.3 Transformer Models Enhancement
- Optimization of relative position embeddings.  
- Improved accuracy in passage ranking.  
- Enhanced question answering capabilities.

### 5.4 Parameter-Efficient Sparse Retrievers
- Implementation of adapters for neural retrieval models.  
- Cost-effective training solutions.  
- Enhanced model efficiency.

### 5.5 Robust Ranker Development
- Multi-adversarial training strategy.  
- Enhanced retrieval efficacy.  
- Integration with existing research.

## 6. Conclusion
The research successfully demonstrates the potential of RAG models in healthcare, combining AI capabilities with medical knowledge access. The model shows promise in accelerating medical knowledge production and understanding while maintaining accuracy and efficiency.

## Additional Notes
This project utilized **RAG** and `mistralai/Mistral-7B-Instruct-v0.1` with **4-bit quantization** on a **Bangladeshi medical dataset** sourced from the Medeasy website. The dataset includes all available drugs in Bangladesh along with their prices, ensuring contextually relevant medicine recommendations for regional diseases.

## References
1. Schumacher, D., Francis, L. J. (2023). V3CTRON Data Retrieval Access System.  
2. RankVicuna: Zero-Shot Listwise Document Reranking.  
3. Transformer Models with Better Relative Position Embeddings.  
4. Parameter-Efficient Sparse Retrievers and Rerankers using Adapters.  
5. Zhou, Y., et al. (2023). Towards Robust Ranker for Text Retrieval.

