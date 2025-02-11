# Detecting Online Abuse: Fine-Tuning LLMs for Abusive Language Detection

This repository contains the code and notebooks for my master's thesis on developing an advanced abuse detection system for online content. The project introduces a novel framework that combines contextual embeddings with sentiment analysis to identify both explicit and subtle forms of online abuse.

## Overview

Online abuse and cyberbullying have become significant challenges on social media platforms, often leading to severe psychological impacts on users. This research presents a new approach to tackle this problem by fine-tuning DistilBERT, integrating sentiment analysis to improve detection accuracy across different forms of abusive content.

### Key Features

- Integration of sentiment analysis with contextual embeddings
- Fine-tuned DistilBERT model for multi-class abuse detection
- Support for detecting six distinct categories of abusive content
- High accuracy in identifying subtle, context-dependent forms of harassment
- Comprehensive evaluation metrics and performance analysis

## System Architecture

The detection framework consists of two main components:

1. **Sentiment Analysis Module**
   - Trained on IMDB movie reviews dataset
   - Extracts emotional context and sentiment features
   - Helps identify subtle and passive-aggressive content

2. **Abuse Detection Module**
   - Fine-tuned DistilBERT architecture
   - Trained on 47,000 annotated tweets
   - Classifies content into six categories:
     - Ethnicity-based abuse
     - Age-based abuse
     - Gender-based abuse
     - Religion-based abuse
     - Other forms of cyberbullying
     - Non-cyberbullying content

## Project Structure

```
.
├── notebooks/
│   ├── Sentiment_Analysis.ipynb
│   └── Cyberbullying_detection_system.ipynb
├── data/
│   ├── imdb_reviews/
│   └── annotated_tweets/
├── requirements.txt
├── LICENSE
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.8+
- CUDA-compatible GPU (recommended)
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ankusharora23/online-abuse-detection.git
cd online-abuse-detection
```

2. Create and activate a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

### Dataset Setup

1. Download the required datasets:
   - Annotated tweets dataset for abuse detection
   - IMDB movie reviews dataset for sentiment analysis

2. Place the datasets in the `data/` directory:
   - `data/imdb_reviews/` for sentiment analysis
   - `data/annotated_tweets/` for abuse detection

## Usage

### Running the Analysis

1. Start with sentiment analysis:
```bash
jupyter notebook notebooks/sentiment_analysis.ipynb
```

2. Run the integrated abuse detection system:
```bash
jupyter notebook notebooks/Cyberbullying_detection_system.ipynb
```

### Model Performance

Our system achieved significant improvements over baseline models:

- Overall accuracy: 85%
- Strong performance across all abuse categories
- Improved detection of subtle forms of abuse
- Enhanced context understanding through sentiment integration

## Research Findings

The integration of sentiment analysis with contextual embeddings has shown remarkable effectiveness in:

- Detecting subtle forms of online abuse
- Reducing false positives in context-dependent cases
- Improving classification accuracy across different abuse categories
- Handling multilingual content effectively

## Contributing

Contributions to improve the system are welcome. Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Citation

If you use this work in your research, please cite:

```bibtex
@mastersthesis{arora2025detecting,
    author = {Arora, Ankush},
    title = {Detecting Online Abuse: Fine-Tuning LLMs for Abusive Language Detection},
    school = {University of Koblenz},
    year = {2025},
    type = {Master's Thesis}
}
```

## Contact

Ankush Arora - [@ankusharora23](https://github.com/ankusharora23)

Project Link: [https://github.com/ankusharora23/online-abuse-detection](https://github.com/ankusharora23/online-abuse-detection)
