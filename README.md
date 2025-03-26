# agriculture_dataset_analysis
## Entity Linking
- [Entity Linking with a Knowledge Base: Issues, Techniques, and Solutions](https://dbgroup.cs.tsinghua.edu.cn/wangjy/papers/TKDE14-entitylinking.pdf)
- [Semantic Search with Knowledge Bases](https://hasibi.com/files/theses/phd-thesis.pdf)

Summary of our planned approach for this project:

**1. Initial Data Processing**
- Contains text data from agricultural news articles
- Need to clean and prepare text data

**2. Text Cleaning**
- Remove special characters if needed
- Handle whitespace and line breaks
- Normalize quotation marks
- Preserve meaningful punctuation
- Maintain sentence structure
- Remove any potential noise/metadata

**3. Topic Modeling**
- Perform before vector database storage
- Topics will be stored as metadata
- Helps with:
  - Document organization
  - Retrieval filtering
  - Understanding content relationships
  - Informing chunking decisions

**4. Text Chunking Strategy**
- Using semantic chunking (rule-based approach)
- No need for fixed-length chunks
- Maintain natural paragraph structures
- Keep related content together
- Preserve quotes and context
- Don't need to worry about uniform chunk sizes

**5. Metadata Structure**
- Will maintain document-chunk relationships
- Each chunk will include:
  - Document ID
  - Chunk ID
  - Date
  - Topic information
  - Other relevant metadata
  - Position/context information

**6. Vector Database Approach**
- Each chunk gets its own embedding
- All embeddings will be same size (determined by model)
- Input text chunks can be different lengths
- Just need to stay within embedding model's token limits
- Store metadata alongside vectors
