# web-crawler-page-rank-simulator
Interactive React simulation for web crawling, text indexing, and PageRank algorithms.
# Web Crawler and Page Ranking Simulator

An interactive, simulation-based educational web application developed for the **Text, Web and Social Media Analytics** subject. It demonstrates how web crawlers discover webpages, how text is processed and indexed, and how search engines rank webpages.

## Overview

Search engines process large amounts of web content to help users find relevant information. This project simulates the core concepts behind this process through a visual, step-by-step interface.

Using a fictional student-resource website, users can explore web crawling, text preprocessing, inverted indexing, PageRank calculation, and keyword-based search without requiring a live internet connection.

## Objectives

- Understand the working of a web crawler.
- Visualize Breadth-First Search (BFS) for webpage discovery.
- Demonstrate text extraction and preprocessing.
- Build an inverted index for efficient keyword lookup.
- Understand PageRank and the influence of incoming links.
- Compare webpage relevance and importance.
- Provide an interactive learning environment for analytics concepts.

## Features

### 1. Web Crawler Simulation
- Visual representation of interconnected webpages.
- Step-by-step crawling process.
- Demonstration of BFS traversal.
- Tracking of visited and discovered pages.
- Crawl depth and event-log visualization.

### 2. Text Processing and Indexing
- Tokenization of webpage content.
- Removal of common stop words.
- Identification of important keywords.
- Construction of an inverted index mapping terms to webpages.

### 3. PageRank Simulation
- Calculation of webpage importance based on link structure.
- Adjustable damping factor and iteration count.
- Comparison of ranking scores across webpages.
- Visualization of PageRank results.

### 4. Search Simulation
- Search using keywords related to student resources.
- Compare keyword relevance and PageRank scores.
- Explore how page content and link structure affect ranking.

### 5. Educational Experiment
- Step-by-step algorithm visualization.
- Sample student-resource webpages.
- Interactive controls.
- Experiment procedure, observations, and conclusion.
- Viva questions for academic preparation.

## Technologies Used

| Technology | Purpose |
|---|---|
| React | User interface and interactive components |
| Vite | Development server and build tool |
| JavaScript | Crawling, indexing, and ranking logic |
| HTML5 | Webpage structure |
| CSS3 | Styling and visualizations |
| Git | Version control |
| GitHub | Source code hosting |

## System Architecture

The simulation follows this conceptual workflow:

```text
Sample Website Graph
        |
        v
   Web Crawler
      (BFS)
        |
        v
  Text Extraction
        |
        v
 Text Preprocessing
(Tokenization and
 Stop-word Removal)
        |
        v
   Inverted Index
        |
        v
  PageRank Algorithm
        |
        v
 Keyword Search and
 Ranking Comparison
        |
        v
 Interactive Results
```

## Algorithms Used

### Breadth-First Search (BFS)

BFS visits webpages level by level, following links from the starting page. A queue is used to manage pages waiting to be visited, while a visited set prevents repeated processing.

### Text Preprocessing

The text-processing stage converts content into searchable terms. Typical operations include lowercasing, tokenization, and stop-word removal.

### Inverted Index

An inverted index stores the webpages associated with each keyword, making it easier to retrieve pages containing a search term.

### PageRank

PageRank estimates webpage importance using the structure of incoming links. The standard iterative formulation is:

\[
PR(A)=\frac{1-d}{N}
+d\sum_{T\in B_A}\frac{PR(T)}{L(T)}
\]

Where:

- \(PR(A)\): PageRank score of page A.
- \(d\): Damping factor, commonly 0.85.
- \(N\): Total number of webpages.
- \(B_A\): Pages linking to page A.
- \(L(T)\): Number of outgoing links from page T.

## Installation and Setup

### Prerequisites

- Node.js installed on your computer.
- npm package manager.
- Git (optional, for cloning the repository).

### Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/AbhiroopKale/web-crawler-page-rank-simulator.git
   ```

2. Navigate to the project directory:

   ```bash
   cd web-crawler-page-rank-simulator
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open the local URL displayed in your terminal, usually:

   ```text
   http://localhost:5173
   ```

## How to Perform the Experiment

1. Open the Web Crawler module.
2. Select the starting webpage.
3. Advance the crawler one step at a time.
4. Observe discovered links, visited pages, and crawl depth.
5. Open the Text Indexing module.
6. Examine how webpage text is tokenized and indexed.
7. Open the PageRank module and adjust its parameters.
8. Compare the resulting PageRank scores.
9. Enter a keyword in the search module.
10. Record the results and explain how page content and link structure affect ranking.

## Expected Results

The experiment is designed to demonstrate that:

- BFS can systematically discover connected webpages.
- Text preprocessing makes webpage content easier to analyze.
- An inverted index supports keyword-based retrieval.
- Pages with influential incoming links can receive higher PageRank scores.
- Keyword relevance and PageRank represent different aspects of search ranking.

Actual observations should be recorded from the simulator's output.

## Limitations

- Uses a predefined, fictional website graph.
- Does not crawl live websites.
- Does not reproduce the complete ranking system of a commercial search engine.
- Uses simplified educational text-processing and search-ranking methods.
- Results depend on the sample webpages, their content, and their links.

## Future Enhancements

- Add live webpage crawling with appropriate permissions.
- Support larger datasets and custom website graphs.
- Integrate TF-IDF or BM25 for improved keyword relevance.
- Add social media text sentiment analysis.
- Compare BFS and Depth-First Search (DFS).
- Export experiment observations and charts as PDF or CSV.
- Deploy the application online for classroom demonstrations.

## Academic Application

**Subject:** Text, Web and Social Media Analytics

**Project Type:** Interactive simulation-based experiment

**Domain:** Web Mining, Information Retrieval, Text Analytics and Search Algorithms

## Author

**Abhiroop Kale**

GitHub: [AbhiroopKale](https://github.com/AbhiroopKale)

## License

This project is intended for educational and academic purposes. A formal open-source license can be added to specify permissions for reuse and distribution.
