# Flowchart

```mermaid
flowchart TD
    A([Start]) --> B([Load Dataset])
    B --> C([Data Cleaning & Preprocessing])
    C --> D([Exploratory Data Analysis])
    D --> E([Feature Engineering])
    E --> F([Model Training & Evaluation])
    F --> G{Is Accuracy Satisfactory?}
    G -- No --> E
    G -- Yes --> H([Select Best Model: Gradient Boosting])
    H --> I([Model Interpretation<br>Classification Report])
    I --> J([Save Model & Results])
    J --> K([Generate Summary Reports])
    K --> L([End / Deployment Ready])