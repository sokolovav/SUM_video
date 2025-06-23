# About

1

# Usage

1

## Parameters:

- `--img_path`: Path to the input image for which you want to generate the saliency map.
- `--condition`: Condition index for generating the saliency map. Each number corresponds to a specific type of visual content:
  - `0`: Natural scenes based on the Salicon dataset (Mouse data).
  - `1`: Natural scenes (Eye-tracking data).
  - `2`: E-Commercial images.
  - `3`: User Interface (UI) images.
- `--output_path`: Path to the folder where the output saliency map will be saved.
- `--heat_map_type`: Type of heatmap to generate. Choose either `HOT` for a standalone heatmap or `Overlay` to overlay the heatmap on the original image.

### Examples

Generate a standalone HOT heatmap for natural scenes images:

```bash
python inference.py --img_path input_image.jpg --condition 1 --output_path output_results --heat_map_type HOT
```

Overlay the heatmap on the original image for e-commerce images:

```bash
python inference.py --img_path input_image.jpg --condition 2 --output_path output_results --heat_map_type Overlay
```

#### Example Images


| Input                                                         | SUM                                                       |
|---------------------------------------------------------------|-----------------------------------------------------------|
| <img src="assets/input.jpg" alt="Original Image" width="300"> | <img src="assets/sum.png" alt="Saliency Map" width="300"> |





### example
<div align="center"> <img src="assets/gradio_demo.png" alt="Gradio Demo" style="width: 80%;"> <p style="font-size: small;">The Gradio interface for SUM Saliency Map Prediction.</p> </div>
