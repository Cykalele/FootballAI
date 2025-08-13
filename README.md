# Amateur End-to-End Football AI – Combined Repository

This repository serves as the **entry point** to the complete FootballAI system.  
It does **not** contain the code of the system itself, but links to the two main repositories:

- **Backend** – [FootballAI_Backend](https://github.com/Cykalele/FootballAI_Backend)  
  Contains the AI-based processing pipeline, tracking, metric computation, and backend server logic.  
  Detailed installation and usage instructions are provided in the backend repository.

- **Frontend** – [FootballAI_UI](https://github.com/Cykalele/FootballAI_UI)  
  Provides the user interface for uploading videos, assigning teams, visualizing metrics, and downloading results.  
  Detailed installation and usage instructions are provided in the frontend repository.

- **Object Detection** – [`object-detection/`](object-detection)  
  Contains the final YOLOv12s-based player, referee, and ball detection configuration developed for the Master's thesis.  
  Includes:
  - Training configuration (`config.yaml`) and YOLO-format class definitions
  - Dataset structure and annotation guidelines ([details](object-detection/dataset/README.md))
  - Training notebook (`train.ipynb`) for the Ultralytics framework
  - Model trained on a combined dataset of own drone footage, penalty-scene images, and broadcast images from Skalski et al.  
  🔗 [View full dataset on Roboflow](https://universe.roboflow.com/footballai-xndiy/masterthesis_dataset)

- **Evaluation** – [`evaluation/`](evaluation)  
  Contains the complete evaluation results and scripts for each system component.  
  - **Object Detection** – [`evaluation/object-detection`](evaluation/object-detection)  
    - `yolo12s_train_val_results`: Graphical results and training logs of the best YOLOv12s model  
    - `yolo12s_test_results_tile`: Evaluation results on the test dataset using tile inference  
    - `train_test_val.ipynb`: Full pipeline including parameter settings and test data evaluation  
  - **Tracking, View Transformation, Team Assignment, Metrics** – individual folders with scripts and results derived from a 6-minute evaluation video ([YouTube link](https://www.youtube.com/watch?v=6_x9rNNgVok&ab_channel=ThomasHauser))  
  - !!Only the object detection evaluation uses a ground-truth test dataset; all other components are evaluated based on persisted outputs from the evaluation video.!!

---

## 📂 Recommended Directory Structure

```plaintext
FootballAI/                 # Main folder
├── FootballAI_Backend/     # Clone from backend repo
├── FootballAI_UI/          # Clone from frontend repo
├── object-detection/       # Training, Test, Validation Data and Configurations
└── evaluation/             # Evaluation results and scripts for all components
```


## 🚀 Getting Started

1. **Create a parent directory and navigate into it**
   ```bash
   mkdir FootballAI
   cd FootballAI
   ```
2. **Clone the backend and frontend repositories**
   ```bash
   git clone https://github.com/Cykalele/FootballAI_Backend.git
   git clone https://github.com/Cykalele/FootballAI_UI.git
   ```
3. **Follow the setup instructions in each repository**
  - [⚙️ Backend Setup Guide](https://github.com/Cykalele/FootballAI_Backend#readme)
  - [🖥️ Frontend Setup Guide](https://github.com/Cykalele/FootballAI_UI#readme)
   





