# TestinderBot_RAG
Retrieval-Augmented Generation Chat for Test Automation and Software Testing: Interactive RAG demo that answers questions about test automation and software testing using the published dataset: Testinder Software Testing &amp; Test Automation Posts (Kaggle).

Quick links
- Kaggle dataset: https://www.kaggle.com/datasets/inderpsingh/testinder-software-testing-and-test-automation-posts
- Notebook (Kaggle): https://www.kaggle.com/code/inderpsingh/testinderbot-rag-p1/

Quickstart (local / Kaggle)
1. Clone the repo and open `TestinderBot_RAG_P1.ipynb`.  
2. Install dependencies:
pip install -r requirements.txt

**Important**: If you install faiss-cpu, restart the kernel / session before running the notebook (to avoid native plugin/CUDA registration warnings).

Run notebook cells from top → bottom. Example query to try in the CLI cell:
How to write a Selenium test to click a button?

What it does
- Loads the published CSV of chunked blog posts.
- Embeds chunks with intfloat/e5-small-v2 and builds a FAISS IndexFlatL2.
- Retrieves top candidates for a user query; optional reranking via cross-encoder/ms-marco-MiniLM-L-6-v2.

Generates final answers using an instruction-tuned generator (FLAN-T5 / Mistral if available).

**Contact**
Author: Inder P Singh
Kaggle Profile https://www.kaggle.com/inderpsingh
YouTube Channel https://youtube.com/c/SoftwareandTestingTraining
AI Blog https://fourth-industrial-revolution.blogspot.com/
Software Testing Blog https://inderpsingh.blogspot.com/

MIT License

Copyright (c) 2025 Inder P Singh

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
1. The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
