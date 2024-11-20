# BrailleCart
**1. Achievements So Far**

**1.1 Grocery Object Detection Using YOLOv8n**
+ Implemented object detection for various grocery items using the YOLOv8n model, achieving a precision of 99.4%.
  
**1.2 Feature Extraction**
+ Extracted relevant features such as brand name and type of product to enhance object recognition accuracy.
  
**1.3 UI Development with Streamlit**
+ Created a basic user interface using Streamlit to facilitate interaction between the visually impaired user and the BrailleCart system.
+ This UI currently allows users to trigger object detection and receive audio feedback.
  
**Current Status of Modules:**
+ Grocery object detection: Fully functional
+ Feature extraction: Fully functional
+ UI using Streamlit: Partially functional
+ OCR integration: Planned for future development
+ LLM-based text-to-speech: Planned for future development
  
**2. Baseline Modules Description**

**2.1 YOLOv8n Object Detection Module**
+ This is the core component of our system, responsible for detecting grocery items from real-time camera input.
+ YOLOv8n was chosen for its accuracy and speed, which is crucial for providing visually impaired users with timely information.
+ This module forms the baseline for all subsequent modules, as accurate item detection is key to the rest of the system functioning effectively.
  
**2.2 Feature Extraction Module**
+ Once an object is detected, the feature extraction module retrieves specific details, such as product brand and type.
+ These details are used by other modules, including OCR and LLM, to provide users with comprehensive information.
  
**2.3 UI (Streamlit-based)**
+ The user interface provides a bridge between the visually impaired user and the BrailleCart system.
+ The UI allows users to initiate object detection and receive feedback in an accessible format.
+ This module's partial functionality currently supports basic interactions, but we plan to enhance it with additional features in upcoming milestones.
  
**3. References**
+ Roboflow Universe, "Grocery Dataset," https://universe.roboflow.com/new-workspace-wfzw3/grocery-dataset-q9fj2/dataset/4
+ Ultralytics, "SKU-110K Dataset," https://docs.ultralytics.com/datasets/detect/sku-110k/
 
**4. Challenges Encountered**

**4.1 OCR Integration**
+ The initial attempt at OCR integration faced issues in detecting labels under different lighting and angle conditions.
+ The quality of the images varied, and the text was often partially obscured, making it difficult for the OCR to extract meaningful information.
  
**4.2 Module Coordination**
+ Integrating various modules (YOLO, OCR, LLM, and UI) and ensuring smooth coordination was challenging.
+ Different latency levels between modules sometimes led to a lag in response time, affecting user experience.
  
**5. Plans to Overcome Challenges**

**5.1 Improving OCR Integration**
+ Plan to experiment with additional OCR tools such as Tesseract and implement preprocessing techniques to enhance image quality.
+ Aiming to make this module more robust by addressing specific issues with text detection under varied lighting conditions.
  
**5.2 Optimizing Module Integration**
+ To address latency, we plan to optimize communication between modules using asynchronous programming and improve computational efficiency.
+ This will involve profiling each component to identify bottlenecks and addressing them appropriately.
  
**5.3 Future Developments**
+ Need to enhance the UI with features such as voice commands and better flow.
+ Need to refine the LLM response generation to provide a more natural and conversational experience.
