# 21_model_comparison
Pricing prediction for cnn models
 Zimbabwe Property Price Predictor
Objective: A multi-modal AI system that predicts property prices using both numerical data and property images.

🏆 Key Results
Best Model: DenseNet

Performance: $255,389 MAE (19.7% better than naive average prediction)

Dataset: 422 properties with images ($50K-$4.2M price range)

Architectures Tested: 20 different neural networks

🚀 Technical Highlights
Inputs: Property features (bedrooms, area, location) + images

Top 5 Models:

DenseNet

SENet

InceptionResNetV2

GoogleNet

Highway Network

Framework: TensorFlow with comprehensive model comparison

📊 Outcome
Successfully identified DenseNet as the optimal architecture for Zimbabwe real estate price prediction, demonstrating the viability of multi-modal deep learning for property valuation despite limited data challenges.

In essence: Built and benchmarked 20 AI models to find the best property price predictor for Zimbabwe market conditions.
opencv-python>=4.5.0
