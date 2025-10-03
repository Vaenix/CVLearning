# Paddle OCR license plate recongnition
## 1 -- Basic Knowledge
## 1.1 Deep Learning
OCR based on deep learning like CNN. It has two tasks, text area positioning and text line recongnition.
## 1.2 Two path
### 1.2.1 Based on Regression
There are also two sub-path, box regression and pixel regression
- For box regression, main methods are CTPN, Textbox and EAST.
    - Advantage: Better results on regular shape text
    - Disadvantage: Can not work accurately on irregular shape
- For pixel regreesion, main methods contain CRAFT and SA-Text.
    - Advantage: Can work on curved text and better on small text
    - Disadvantage: Insufficient real-time performance
### 1.2.2 Based on Segmentation
This method is not limited by the shape, but more after process makes higher power cost.
However, some algorithm such as DB handle this issue.
## 1.3 Main method
There are many methods, no more word to explan. 
One table for comparsion

### OCR Methods Comparison

| Method   | Core Advantages                         | Applicable Text Types                         |
|----------|-----------------------------------------|-----------------------------------------------|
| Rosetta  | Lightweight, multilingual support       | Social media images, multilingual texts       |
| CRNN     | Classic architecture, strong robustness | Printed text, simple handwriting              |
| STAR-Net | Spatial attention mechanism             | Complex backgrounds, curved texts             |
| RARE     | Automatic rectification of deformed text| Transparent/curved texts (e.g., advertisements)|
| SRN      | Semantic reasoning, global context      | Long texts, documents                         |

