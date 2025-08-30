# Agri-Sense AI: Satellite Crop Health Monitor

An AI-powered platform for early detection of crop stress and disease from satellite imagery, promoting sustainable agriculture.

## 🌟 The Story & Inspiration

The inspiration for this project came from a deep-seated desire to create a solution that tackles a real-world, high-impact problem in India. We focused on the agricultural sector, where timely information can mean the difference between a successful harvest and crop failure. By leveraging the power of satellite imagery and deep learning, we aimed to build a tool that could provide farmers with a vital early warning system for crop health issues.

## ✨ Features

- **Satellite Data Processing:** Automated pipeline to ingest and process multispectral satellite imagery from Sentinel-2.
- **NDVI Calculation:** Computes the Normalized Difference Vegetation Index (NDVI) to quantify crop health.
- **Deep Learning Model:** A Convolutional Neural Network (CNN) trained to classify crop health into categories like `healthy`, `stressed`, and `diseased`.
- **Health Mapping:** Generates clear, color-coded health maps for easy visualization and analysis.
- **Data-Driven Insights:** Provides key statistics on crop health and trends over time.

## 🛠️ Built With

* **Languages:** Python, SQL
* **Deep Learning:** TensorFlow, Keras
* **Data Analysis:** pandas, numpy, `rasterio` (for geospatial data)
* **Visualization:** Matplotlib, Seaborn
* **APIs & Platforms:** Kagglehub, Copernicus Open Access Hub
* **Cloud Services:** Google Colab
* **Version Control:** Git

## 📈 Methodology

Our approach combines geospatial data processing with a deep learning model. First, we use `rasterio` to read raw satellite imagery from Sentinel-2. The core of our analysis is the NDVI, a metric derived from the Near-Infrared (NIR) and Red spectral bands. The formula is as follows:

$$NDVI = \frac{(NIR - Red)}{(NIR + Red)}$$

This NDVI data, along with other spectral bands, is then used as input for our CNN, which is trained to predict crop health at a granular, pixel level.

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

* Python 3.8+
* pip

### Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/agri-sense-ai.git](https://github.com/your-username/agri-sense-ai.git)
    ```
2.  Navigate to the project directory:
    ```bash
    cd agri-sense-ai
    ```
3.  Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

1.  Download a Sentinel-2 satellite image for your area of interest.
2.  Place the `.tif` band files in the `data/raw` directory.
3.  Run the main processing script to generate predictions and health maps.

## 🤝 Challenges & Learnings

The biggest challenge was handling the sheer size and complexity of satellite data. Learning to filter out images with heavy cloud cover and efficiently process the large multi-band files was a major hurdle. This project taught me the importance of data preprocessing in a deep learning pipeline, and how to adapt standard ML workflows to a specialized domain like geospatial analysis.


