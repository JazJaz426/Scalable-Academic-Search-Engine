# Distributed Search System – Scalable Academic Search Engine
A MapReduce-based distributed search engine designed for efficiently discovering and indexing academic papers from Usenix conferences. This system leverages parallel processing and distributed computing to handle large-scale datasets, improving search accuracy and retrieval speed.

# Features
- Web Crawler – Iteratively collects URLs of academic papers.
- Downloader – Fetches and preprocesses text from crawled URLs.
- Indexer – Builds an inverted index for fast and efficient querying.
- Querier – Retrieves relevant academic papers based on search terms, ranking results by relevance.
- Scalable Deployment – Optimized for AWS EC2 instances, enabling dynamic scaling.
- Performance Optimizations – Implements batch processing, network traffic reduction, and serialization improvements to enhance efficiency.

# Challenges & Solutions
- Socket Hang-Ups – Resolved by implementing batch processing to reduce coordination overhead.
- Serialization Errors – Special character filtering ensures clean data handling.
- Load Balancing – Investigating hashing improvements for better task distribution across nodes.
- 
# How to Use
Run Crawler: `npm run test test/crawlv3.test.js`
Download Text: `npm run test test/downloadText.test.js`
Index Data: `npm run test test/invert.test.js`
Query Papers: `npm run test test/query.test.js`

# Future Improvements
- Implement breadth-first search crawling with cycle detection.
- Enhance parallel downloading and adaptive bandwidth management.
- Optimize indexing with advanced NLP techniques for better academic term recognition.
