# CampusGuard-AI
CampusGuard AI – Real-Time Weapon Detection

## Notebook used in Data Analysis and Model Building
[campusguardai.ipynb]([https://github.com/AbelEsther/CampusGuard-AI.ipynb](https://github.com/AbelEsther/CampusGuard-AI/blob/main/CampusGuard_AI_group6.ipynb)

## Dataset Link
[campusguardai.csv]([https://github.com/AbelEsther/CampusGuard-AI.csv](https://drive.google.com/file/d/1QMQDV9G8-uN20-YIaw_y3R88vyYNPzR8/view?usp=sharing)


## **Problem/opportunity definition**
Campus safety is a top priority at Arizona State University (ASU), especially with recent nighttime incidents involving weapons near campus. This project aims to develop a real-time, scalable weapon detection system that can strengthen real-time situational awareness, enhance the efficiency of existing security infrastructure, and set a precedent for AI-driven campus safety solutions across universities nationwide.

## **Why is this important to solve**
Incidents involving weapons near campus threaten the safety of students, faculty, and staff. Traditional security methods are often reactive and slow to detect threats. ASU's real-time, AI-powered weapon detection system enables a proactive approach to prevent incidents before they escalate.

## **Who are the stakeholders and beneficiaries**
- ASU Police Department
- Students
- Faculty and Staff
- Campus Security and IT
- University Leadership

## **How is it being solved today and what are the issues**
The ASU Police Department ensures campus safety through patrols and community engagement, but traditional surveillance is reactive and often delayed. Manual systems may miss emerging threats, especially in remote or low-traffic areas, limiting early prevention.

## **Proposed end-to-end product solution idea and why the CV component is essential to the solution**
-	**Dataset:** Weapon Dataset from Roboflow Universe with 896 images of weapons https://universe.roboflow.com/spot-ai/spot-ai-zbxjw
-	**YOLOv8 Object Detection Model:**  Identifies visible weapons like guns or knives in real-time
-	**Threat Classification & Logging:** Based on confidence levels
-	**Immediate Alert System:**  When integrated into the live feed of the ASU webcam, it sends a notification to the security team (SMS, email, dashboard).

## **Why Computer Vision is Core:**
- Detects visual objects (weapons) in milliseconds
- Works 24/7 without fatigue or blind spots
- Scales across hundreds of camera feeds
- Adapts to day/night and indoor/outdoor settings

## **Possible limitations/risks**
1.	Real-time processing may be hardware-intensive
2.	Mistaking harmless items (e.g., phones, tools) for weapons (False Positives)
3.	May require ASU IRB approval or administrative review if used in actual deployment

---

## **Data Source**
- **Dataset:** DaSCI dataset, containing annotated images classified into two categories: guns and human objects.
- **Size:** <1GB, making it lightweight and efficient for processing.
- **Preprocessing:** Images are resized to 500 pixels for faster model inference.

## **Model Training**
- **Framework:** Python-based YOLOv8 (You Only Look Once), a state-of-the-art object detection model.
- **Approach:**
  - Image annotation with bounding boxes.
  - Confidence threshold tuning for accuracy.
  - Iterative testing to refine detection capabilities.
           
----
## **Testing & Performance Evaluation**
- The model is validated using multiple testing approaches.
-  Performance metrics include precision, recall, and confidence levels.
-  Edge cases are handled through data augmentation and model fine-tuning.

## **Deployment**
- The project is open-source and available on GitHub for further enhancement.
-  Potential applications include academic research, law enforcement, and public surveillance systems.

## **Deliverable**:
- Final Output: An efficient weapon detection model visually identifying firearms in public spaces. 
- The system utilizes a pre-trained Haar Cascade Object Detection Model for additional verification.
- Visualization: The detected weapon is highlighted with bounding boxes in real-time.

---
### **How to Run the Project**
a. **Clone the repository:**
  - git clone https://github.com/your-repo/campusguardai.git
  - cd ironsight
  
b. **Install dependencies:**
   - pip install -r requirements.txt

c. **Run the detection script:**
   - python detect.py --source test_images/

---
### d. **Contributors - Team 6 Members**
1. [Esther Abel](https://www.linkedin.com/in/abelesther/)
2. [Aishwarya Jadeja](https://www.linkedin.com/in/aishwarya-jadeja-5729282a8/)
3. [Dhrushi Padma](https://www.linkedin.com/in/dhrushi-padma-09abb623b/)
4. [Haarika Atluri]()
5. [Nayana Hegde](https://www.linkedin.com/in/nayana-hegde-501a7785/)

## **Acknowledgment**
We appreciate the effort of the team and our Prof. Hina for this project, as well as the DaSCI dataset, for making this project possible.

**Thank You!**
---
If you would like more details, you can visit our GitHub repository.


