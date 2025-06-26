 a real-time surveillance application that:

Detects threats or key objects (like weapons, humans, vehicles) using YOLO.
Classifies scene types (e.g., indoor, outdoor, day, night) using a ResNet classifier.
Stylizes safe or archival footage into binary or artistic forms (e.g., sketch, thermal-style, stencil) using a custom Neural Style Transfer model trained for binary artistic rendering.
Essentially: Smart object detection + environment classification + real-time artistic binary stylization


🧰 Tech Stack:
TensorFlow 2.x
OpenCV (for webcam/video processing)
YOLOv8 via TensorFlow (or ported)
ResNet from tf.keras.applications
Custom Style Transfer model (with binary/sketch stylization)
Flask or Streamlit for a live dashboard (optional but impactful)



🧪 Example Use Case:
A smart CCTV system deployed in a museum:
Detects suspicious actions (YOLO).
Classifies environment for lighting conditions (ResNet).
If abnormal is detected — it stores an artistic, binary-style version of the footage for efficient archival (NST).
Threat frames are stored in raw RGB + highlighted bounding boxes.
