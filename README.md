# Image Clustering and Pixel Segmentation

This project converts an image into pixel-level data, explores image cleaning, and compares clustering approaches for image segmentation. The repository includes the original assignment notebooks, a polished rainbow project notebook, a GPT-vs-other comparison notebook, and the final PDF report.

## Project Files

- `Image_Clustering_and_Pixel_Segmentation.ipynb` - polished rainbow image clustering notebook
- `GPT_and_Other_Comparison.ipynb` - comparison notebook for the GPT-assisted and other versions
- `homework2.ipynb` - original homework notebook
- `homework2_.ipynb` - alternate/non-GPT homework notebook
- `homework2_ans.ipynb` - completed answer notebook
- `homework2_gpt.ipynb` - GPT-assisted homework notebook
- `Dam_final_report.pdf` - final written report with the updated project title
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

Open `Image_Clustering_and_Pixel_Segmentation.ipynb` directly on GitHub for the main project. GitHub will render the notebook with its markdown, code cells, and saved outputs.

Open `GPT_and_Other_Comparison.ipynb` to compare the GPT-assisted notebook with the other submitted versions.

## How to Run Locally

1. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Place the input image `rainbow.jpg` in the same folder as `Image_Clustering_and_Pixel_Segmentation.ipynb`.

3. Open the notebook:

   ```bash
   jupyter notebook Image_Clustering_and_Pixel_Segmentation.ipynb
   ```

## Note

The polished notebook references `rainbow.jpg` as the source image. That image was not present in the original project folder when this GitHub-ready folder was created, so it must be added before rerunning the notebook from the beginning.

Project completed by: Dhwani Patel
