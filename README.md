# Image Analysis and Clustering

This project converts an image into pixel-level data, explores image cleaning, and compares clustering approaches for image segmentation. The main deliverable is a Jupyter notebook that walks through the full workflow from image loading to visualization.

## Project Files

- `Project_DAM.ipynb` - main Jupyter notebook for the analysis
- `Dam_final_report.pdf` - final written report
- `assets/` - preview images used in this README
- `requirements.txt` - Python packages used by the notebook

## Methods Used

- Image loading and RGB pixel extraction with Pillow and NumPy
- Pixel dataset creation with pandas
- Image visualization and noise filtering with matplotlib
- KMeans clustering with scikit-learn
- Custom clustering implementation with PyTorch
- Cluster visualization with seaborn and matplotlib

## Input and Results Preview

The notebook begins by converting the input image into a pixel dataset with RGB values and x/y coordinates.

```text
    R   G   B  x  y
0  68  67  49  0  0
1  42  43  27  1  0
2  43  43  31  2  0
3  34  35  27  3  0
4  50  49  44  4  0
```

| Input Image | Cleaned Image |
| --- | --- |
| ![Original rainbow image](assets/original_image.png) | ![Cleaned rainbow image](assets/cleaned_image.png) |

| scikit-learn KMeans Result | Custom PyTorch Clustering Result |
| --- | --- |
| ![KMeans clustered image](assets/sklearn_clustered_image.png) | ![PyTorch clustered image](assets/pytorch_clustered_image.png) |

| Cluster Distribution | PCA Cluster Plot |
| --- | --- |
| ![Cluster distribution plot](assets/sklearn_cluster_distribution.png) | ![PCA cluster plot](assets/pca_cluster_plot.png) |

## How to View

Open `Project_DAM.ipynb` directly on GitHub. GitHub will render the notebook with its markdown, code cells, and saved outputs.

## How to Run Locally

1. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Place the input image `rainbow1.jpg` in the same folder as `Project_DAM.ipynb`.

3. Open the notebook:

   ```bash
   jupyter notebook Project_DAM.ipynb
   ```
