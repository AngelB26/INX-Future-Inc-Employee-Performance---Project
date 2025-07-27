flowchart TD
    %% Start Point
    A([Start]) --> B([Load Dataset])

    %% Data Preparation Phase
    B --> C([Data Cleaning & Preprocessing])
    C --> D([Exploratory Data Analysis])
    D --> E([Feature Engineering])

    %% Modeling Phase
    E --> F([Model Training & Evaluation])
    F --> G{Is Accuracy Satisfactory?}

    %% Decision Loop
    G -- No --> E
    G -- Yes --> H([Select Best Model: Gradient Boosting])

    %% Post-Modeling Phase
    H --> I([Model Interpretation<br>Classification Report])
    I --> J([Save Model & Results])
    J --> K([Generate Summary Reports])

    %% End Point
    K --> L([End / Deployment Ready])
