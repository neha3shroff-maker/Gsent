## License
This dataset is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to share and adapt the dataset, provided you give appropriate credit by citing the following:

Neha Shah. (2025). Gujarati Sentiment Dataset (GSent-105K) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.17189396


# GSent-88K: Gujarati News Headlines Sentiment Dataset

## Dataset Description
GSent-88K is a large-scale dataset of Gujarati news headlines annotated for sentiment: positive, negative, and neutral.  

- **Full dataset**: 88,800 semi-manual annotations  
- **Manual subset**: 11,625 fully manually annotated headlines for quality validation  

The dataset provides **text-only sentiment labels**, making it suitable for training and benchmarking sentiment analysis models in Gujarati, a low-resource language.

---

## Columns
- `Headline`: Gujarati news headline  
- `Label`: Sentiment (-1 = Negative, 0 = Neutral, 1 = Positive)  

---

## Annotation Guidelines
- **Positive**: Headlines expressing positive sentiment or praise  
- **Negative**: Headlines expressing criticism, concern, or negative sentiment  
- **Neutral**: Informative or factual headlines with no clear sentiment  

---

## Versioning
- v1.0 semi-manual: Full semi-automated annotations  
- v1.0 manual: Gold-standard manually annotated subset  

---

## License
**CC-BY 4.0 (Attribution)** – You are free to use, share, and modify this dataset for research purposes. Please provide proper citation.

---

## Citation

If you use this dataset, please cite it as:

Neha Shah. GSent-88K: A Large-Scale Gujarati News Headlines Sentiment Dataset. Zenodo, v1.0. DOI: [10.5281/zenodo.17189396](https://doi.org/10.5281/zenodo.17189396)

---

## Examples
| Headline | Label |
|----------|-------|
| “ગુજરાતમાં શાળાઓ ફરી ખોલાય છે” | 1 |
| “મહામારીને કારણે બજારો બંધ છે” | -1 |
| “રાજ્ય સરકારનું નવું બજેટ જાહેર” | 0 |

---

## How to Use
Load in Python using pandas:

```python
import pandas as pd

# Full dataset
full = pd.read_csv('data/GSent88K_full.csv', encoding='utf-8-sig')

# Manual subset
manual = pd.read_csv('data/GSent88K_manual.csv', encoding='utf-8-sig')
