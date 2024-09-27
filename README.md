# Beyond Buzzwords: NLP Reveals Common Threads in Sustainable and Circular Construction Discourse

## Overview
This repository contains the code and data for the paper **"Beyond Buzzwords: NLP Reveals Common Threads in Sustainable and Circular Construction Discourse."** The study explores the differences and overlaps between "Circular Economy" and "Sustainability" within the context of the construction sector, using Natural Language Processing (NLP) techniques to analyze a large dataset of academic literature. 

The analysis employs three NLP methods—TextRank, TF-IDF, and Concept Matrix—applied to a dataset of 480 academic papers to discover thematic and conceptual patterns. The findings offer insights into the specific focus of circular construction on resource efficiency and waste management, as well as the broader scope of sustainable construction, which includes urban planning, community development, and long-term environmental impacts.

## Repository Contents

This repository is organized into several Jupyter Notebooks that represent the different methods used in the study:

- **[ConceptMatrix.ipynb](./notebook/ConceptMatrix.ipynb)**:  
  Implements the Concept Matrix approach to discover contextual associations between key terms in the dataset, revealing how circular construction is more operational and sector-specific compared to sustainable construction.

- **[Clustering.ipynb](./notebook/Clustering.ipynb)**:  
  Contains code for clustering the dataset based on the terms found using NLP methods, providing a clear visual representation of how different concepts are grouped within the literature.

- **[Evaluation_Methods.ipynb](./notebook/Evaluation_Methods.ipynb)**:  
  Includes the evaluation metrics used to assess the performance and relevance of the NLP methods in identifying key themes in the literature.

- **[TextRank_approach.ipynb](./notebook/TextRank_approach.ipynb)**:  
  Applies the TextRank algorithm to reveal the relationships between circular economy and sustainability concepts, showing the nested nature of circular economy principles within broader sustainability goals.

- **[TFIDF_approach.ipynb](./notebook/TFIDF_approach.ipynb)**:  
  Demonstrates the use of the TF-IDF method to differentiate between the targeted approach of circular construction and the more comprehensive nature of sustainable construction.

## Dataset

The dataset used in this study consists of 381 academic papers focused on the topics of "Circular Economy" and "Sustainability" in the construction sector. 

- **Data Files**:
  - **CE_SC_papers.csv**: Contains original raw data (381 papers) with following features: author; title; abstract; article_text_string; article_text_list; number_of_symbols; number_of_words; number_of_sentences.
  - **articles_for_term_extraction.csv**: Contains the filtered data of the 375 papers.
  - **common_text_rank_terms.csv** and **common_tfidf_terms.csv**: Lists of common terms identified using TextRank and TF-IDF.
  - **unique_CE_text_rank_terms.csv**, **unique_CE_tfidf_terms.csv**, **unique_SC_text_rank_terms.csv**, and **unique_SC_tfidf_terms.csv**: Lists of unique terms for Circular Economy (CE) and Sustainability in Construction (SC) derived from TextRank and TF-IDF analyses.
  - **groups.txt**: Text file delineating the methodological grouping of the papers.
  - **wikifier.pkl**: Pickled file containing data processed through Wikifier for enhanced term recognition and linking.

## Requirements

To run the notebooks in this repository, you will need the following Python packages:

- `pandas`
- `numpy`
- `scikit-learn`
- `nltk`
- `matplotlib`
- `networkx`
- `gensim`

To install the required dependencies, you can run:

```bash
pip install -r requirements.txt
```

## How to Use the Notebooks

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AlexPak/paper-2024-nu-sustainable-constr.git
   cd paper-2024-nu-sustainable-constr
   ```

2. **Install the dependencies** by running the provided `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebooks**:
   Open each notebook in Jupyter and run the cells in sequence. Each notebook includes markdown cells with explanations of the methods, outputs, and interpretations.

   - **ConceptMatrix.ipynb**: Run this notebook to analyze key term associations using the Concept Matrix.
   - **Clustering.ipynb**: Run this notebook to visualize the clusters formed based on the literature's thematic similarities.
   - **Evaluation_Methods.ipynb**: Evaluate the performance of each NLP method used in this study.
   - **TextRank_approach.ipynb**: Explore how TextRank reveals relationships between circular economy and sustainability concepts.
   - **TFIDF_approach.ipynb**: See how TF-IDF is used to differentiate between circular construction and sustainable construction.

## Results

The primary results of this study include:

1. **Circular construction** is more operationally focused, emphasizing resource efficiency, waste management, and recycling processes specific to the construction industry.
   
2. **Sustainable construction** is more comprehensive and incorporates aspects like urban planning, long-term environmental impacts, and community development.

3. **TextRank and TF-IDF** effectively differentiate these themes, while the **Concept Matrix** reveals the contextual associations of key terms and emphasizes the practical focus of the circular economy.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgment
This work was supported by the Ministry of Education and Sciences of the Republic of Kazakhstan under the following grant #AP14871214. The funders had no role in study design, data collection and analysis, decision to publish, or preparation of the manuscript. The authors acknowledge the financial support from the Nazarbayev University Faculty Development Competitive Research Grant Program (Funder Project Reference: 20122022CRP1606).

## Citation

If you use this code or dataset for your research, please cite the corresponding paper:

**Author(s)**: 
Shakarim Aubakirov, Kazakh-British Technical University, Almaty, Kazakhstan
Aleksandr Pak, Kazakh-British Technical University, Almaty, Kazakhstan
Iskander Akhmetov, Kazakh-British Technical University, Almaty, Kazakhstan
Aidana Tleuken, Nazarbayev University, Astana, Kazakhstan
Huseyin Atakan Varol, Institute of Smart Systems and Artificial Intelligence, Astana, Kazakhstan
Assel Akzhalova, Kazakh-British Technical University, Almaty, Kazakhstan
Ferhat Karaca, Nazarbayev University, Astana, Kazakhstan
  
**Title**: *Beyond Buzzwords: NLP Reveals Common Threads in Sustainable and Circular Construction Discourse*  
**Journal**: PeerJ Computer Science  
**Year**: 2024  
**DOI**: [Add DOI once available]

