# 21_model_comparison
Pricing prediction for cnn models
# Zimbabwe Property Price Prediction

A multi-modal deep learning system that predicts property prices in Zimbabwe using both tabular features and property images. The project evaluates 20 different neural network architectures to find the optimal model for real estate valuation.

## 🏆 Model Performance

### Best Performing Model: **DenseNet**
- **MAE**: $255,389.37
- **R²**: -0.004
- **Improvement over naive predictor**: +19.7%

### Top 5 Models by MAE:
1. **DenseNet** - MAE: $255,389.37 | R²: -0.004
2. **SENet** - MAE: $272,636.92 | R²: -0.122
3. **InceptionResNetV2** - MAE: $280,589.37 | R²: -0.240
4. **GoogleNet** - MAE: $295,502.56 | R²: -0.039
5. **Highway** - MAE: $301,804.41 | R²: 0.010

## 📊 Dataset

### Original Data
- **Total properties**: 1,613
- **Features**: 15 columns including price, location, bedrooms, bathrooms, areas, etc.
- **Unique locations**: 38

### Cleaned Data
- **After outlier removal**: 1,371 properties
- **Price range**: $50,000 - $5,000,000
- **Removed outliers**: 242 properties (15.0%)

### Final Training Data
- **Properties with valid images**: 422
- **Training set**: 337 samples
- **Test set**: 85 samples
- **Average price**: $502,125

## 🏗️ Model Architectures Evaluated

The project tested 20 different neural network architectures:

1. AlexNet
2. NIN (Network In Network)
3. ZFNet
4. VGG
5. GoogleNet
6. InceptionV3
7. Highway Network
8. InceptionV4
9. ResNet
10. InceptionResNetV2
11. FractalNet
12. WideResNet
13. Xception
14. Residual Attention Network
15. SENet (Squeeze-and-Excitation Network)
16. DenseNet 🏆
17. CompetitiveSENet
18. MobileNetV2
19. CapsuleNet
20. HRNetV2

## 🔧 Features

### Tabular Features Used:
- Building area
- Land area
- Number of bedrooms
- Number of bathrooms
- Image count
- Price per square meter
- Area ratio (building/land)
- Room density
- Location (encoded)

### Image Processing:
- Image size: 224×224×3
- Preprocessing: RGB conversion, resizing, normalization
- Image mapping between CSV filenames and actual image files

### Feature Engineering:
- Price per square meter
- Area ratio calculations
- Room density metrics
- Location encoding

## 🚀 Installation

```bash
# Clone repository
git clone https://github.com/yourusername/zimbabwe-property-predictor.git
cd zimbabwe-property-predictor

# Install dependencies
pip install -r requirements.txt
