**Object Detection WebApp**

This project implements an **object detection application** using PyTorch's **Faster R-CNN with ResNet-50 FPN** as the detection model. It is wrapped in a user-friendly **Streamlit** interface for easy image uploads and visualization of detection results.




## Features  
- Detects objects in images using **Faster R-CNN pretrained on the COCO dataset**.  
- Displays bounding boxes and labels on detected objects.  
- **Streamlit dashboard** for uploading images and viewing predictions.  
- High configurability with adjustable confidence thresholds.  
- Supports a wide range of object categories from the COCO dataset (e.g., "person," "car," "dog," etc.).  


## Installation  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/object-detection-app.git
   cd object-detection-app
   ```

2. **Set Up a Python Environment**  
   - It’s recommended to use a virtual environment:
     ```bash
     python -m venv env
     source env/bin/activate  # On Windows: env\Scripts\activate
     ```

3. **Install Dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the App**  
   ```bash
   streamlit run object_detection_app.py
   ```

5. **Access the App**  
   - Open your browser and navigate to the URL displayed in your terminal (usually `http://localhost:8501`).

---

## How It Works  

1. **Model Loading**:  
   - The app uses **Faster R-CNN with ResNet-50 FPN**, pretrained on the **COCO dataset**.  
   - The pretrained weights are automatically downloaded by PyTorch.  

2. **Image Preprocessing**:  
   - Images are normalized and resized to match the COCO training format.  

3. **Object Detection**:  
   - The model detects objects and returns bounding boxes, labels, and confidence scores.  

4. **Visualization**:  
   - Bounding boxes and labels are drawn on the image and displayed on the Streamlit app.  

---

## Supported Categories  

This application supports **90 object categories**, including:  
- **Vehicles**: Car, Bus, Bicycle, Truck, etc.  
- **People**: Person  
- **Animals**: Dog, Cat, Bird, etc.  
- **Household Items**: Chair, Couch, Refrigerator, etc.  

For the full list of categories, refer to the COCO dataset's [official site](https://cocodataset.org/#home).

---

## Example Usage  

1. **Upload an Image**:  
   - Use the file uploader to upload an image in `png`, `jpg`, or `jpeg` format.  

2. **View Results**:  
   - The app displays the image with bounding boxes and a table of detected objects with their confidence scores.  

---

## Dependencies  

The project requires the following Python packages:  

- **streamlit**  
- **torch**  
- **torchvision**  
- **pillow**  
- **matplotlib**  
- **numpy**  


## Acknowledgments  

- Pretrained models: [PyTorch Model Hub](https://pytorch.org/vision/stable/models.html)  
- COCO Dataset: [COCO Dataset](https://cocodataset.org/)  
- Streamlit for UI: [Streamlit](https://streamlit.io/)  


## License  

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.


Let me know if you’d like to customize this further! 😊
