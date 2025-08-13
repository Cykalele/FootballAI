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

---

## 📂 Recommended Directory Structure

```plaintext
FootballAI/                 # Main folder
├── FootballAI_Backend/     # Clone from backend repo
└── FootballAI_UI/          # Clone from frontend repo
└── Object-Detection/       # Storage of Training, Test, Validation Data and Configurations
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
   





