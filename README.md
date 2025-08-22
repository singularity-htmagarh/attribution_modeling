# Attribution Modeling

This folder is part of the [`Marketing_Science_Projects`](https://github.com/singularity-htmagarh/Marketing_Science_Projects) repository and focuses on **Attribution Modeling** – a set of techniques for analyzing and assigning credit to marketing touchpoints in the customer journey.

## Table of Contents

- [Overview](#overview)
- [Folder Structure](#folder-structure)
- [Features & Methods](#features--methods)
- [How to Use](#how-to-use)
- [Requirements](#requirements)
- [Usage Examples](#usage-examples)
- [Customization](#customization)
- [Contributing](#contributing)
- [References](#references)
- [License](#license)

---

## Overview

Attribution modeling is critical in digital marketing analytics, helping brands understand how different channels (such as email, social, paid search, etc.) contribute to conversions. This project provides code, templates, and documentation for applying popular attribution models, including:

- First-touch
- Last-touch
- Linear
- Time-decay
- Position-based (U-shaped)
- Data-driven/custom models

The goal is to provide an extensible foundation for marketers and data scientists to experiment, evaluate, and deploy attribution models.

---

## Folder Structure

```
attribution_modeling/
├── data/               # Sample datasets for touchpoint and conversion tracking
├── notebooks/          # Jupyter/Colab notebooks for interactive analysis
├── scripts/            # Python scripts for attribution calculations
├── utils/              # Utility/helper functions
├── results/            # Output reports and model results
├── requirements.txt    # Python dependencies
└── README.md           # Documentation (this file)
```

---

## Features & Methods

- **Preprocessing**: Load, clean, and format multi-channel marketing data.
- **Attribution Algorithms**: Implementation of standard and customizable models.
- **Visualization**: Summarize and visualize channel contributions.
- **Reporting**: Export results to CSV, Excel, or dashboards.
- **Extensibility**: Easily add new models or input data sources.

### Attribution Models Supported

| Model Type          | Description                                           |
|---------------------|------------------------------------------------------|
| First-Touch         | Assigns all credit to the first channel              |
| Last-Touch          | Assigns all credit to the last channel               |
| Linear              | Equal credit to all touchpoints                      |
| Time-Decay          | More credit to recent touchpoints                    |
| Position-Based      | Weighted: most credit to first & last, rest split    |
| Data-Driven         | Custom/ML-based; learns from conversion patterns     |

---

## How to Use

1. **Clone Repository**

   ```sh
   git clone https://github.com/singularity-htmagarh/Marketing_Science_Projects.git
   cd Marketing_Science_Projects/attribution_modeling
   ```

2. **Install Dependencies**

   ```sh
   pip install -r requirements.txt
   ```

3. **Prepare Data**

   - Place your multi-touchpoint data (CSV, Excel) in the `data/` folder.
   - Ensure columns include: `user_id`, `touchpoint`, `channel`, `timestamp`, `conversion`.

4. **Run Attribution Models**

   - Use Jupyter notebooks in `notebooks/` for interactive analysis.
   - Or run scripts from the `scripts/` directory.

---

## Requirements

- Python 3.8+
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn (see `requirements.txt` for details)
- Jupyter Notebook (recommended for interactive exploration)

---

## Usage Examples

### 1. Interactive Notebook

Open `notebooks/attribution_analysis.ipynb` and run cells to:

- Load data
- Apply attribution models
- Visualize results

### 2. Command-Line Script

```sh
python scripts/attribution_linear.py --input data/sample_touchpoints.csv --output results/linear_results.csv
```

---

## Customization

- **Add New Models**: Create new scripts in `scripts/` or functions in `utils/`.
- **Change Weights**: Edit parameters for position-based or time-decay models in relevant scripts.
- **Input Data**: Format your data as per sample files in `data/`.

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements, bug fixes, or new features.

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## References

- [Google Analytics Attribution Models](https://support.google.com/analytics/answer/1662518?hl=en)
- [Data-Driven Attribution](https://www.analyticsvidhya.com/blog/2020/10/what-is-marketing-attribution-models/)
- [Multi-Touch Attribution with Python](https://towardsdatascience.com/multi-touch-attribution-models-in-python-2b81a7b7e4c2)

---

## License

Distributed under the MIT License. See [`LICENSE`](../LICENSE) for more information.

---

> For questions, reach out to [@singularity-htmagarh](https://github.com/singularity-htmagarh)
