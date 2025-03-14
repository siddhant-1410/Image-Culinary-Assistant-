# Image-Based Culinary Assistant

> **Note:** A demo video will be uploaded once the project is fully completed. Further enhancements and additions are outlined in the last section of this document.

The **Image-Based Culinary Assistant** is an AI-powered application that helps users discover recipes based on food images. By leveraging **computer vision**, the app identifies food items from uploaded images and generates a recipe accordingly.

> **Development Status:** The project is under development and is expected to be completed by the **first week of April**.

## Techniques Used

- **Data Augmentation & Preprocessing:** Applied transformations like **rotation, shifting, zooming, and flipping** using `ImageDataGenerator`.
- **CNN Architecture:** Utilized multiple `Conv2D` layers with `LeakyReLU`, **Batch Normalization, MaxPooling, and GlobalAveragePooling2D**.
- **Regularization & Optimization:** Implemented **Dropout, L2 regularization, Adam optimizer, and class weighting** to handle imbalance.
- **Training Enhancements:** Used **Early Stopping and ReduceLROnPlateau** to prevent overfitting and optimize learning rates.

## Retrieval-Augmented Generation (RAG)

The project implements **RAG** to enhance recipe generation by retrieving relevant recipe content from indexed PDFs.

## Features

- **Dish Classification:** A CNN model trained on **25 Indian dishes** to classify the uploaded food image.
- **Text Extraction:** Extracts text from **recipe PDFs** using `pdfplumber`.
- **Vector Search (FAISS):** Embeds and indexes recipes for **efficient retrieval**.
- **Recipe Generation:** Utilizes the **Google Gemini API** to generate well-structured recipes.

## Technologies Used

- **Machine Learning & Deep Learning:** `TensorFlow`, `OpenCV`, `SentenceTransformers`
- **Text Processing:** `pdfplumber`
- **Vector Search:** `FAISS`
- **AI API:** `Google Gemini API`

## Usage

1. **Place** recipe PDFs in the `recipes_pdf` folder.
2. **Run** the script with an **image path** to classify the dish and retrieve its recipe.
3. The system will **generate a well-structured, step-by-step recipe** based on the extracted content.

## Future Updates

- **Recommender System:** The system will incorporate a **recommender system** to suggest similar dishes based on the uploaded image.
- **Language Translator:** A **language translation model** will be developed from scratch using an **encoder-decoder architecture**, enabling the translation of recipes from **English to Hindi**.
