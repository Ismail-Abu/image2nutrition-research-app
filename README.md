# image2nutrition-research-app
A mobile app that analyzes food images and breaks down nutritional content into RAG/SAG categories for protein, fats, and calories. This is built for research and usability.

## Overview

This project explores whether it's possible to accurately break down a food image into its nutritional facts using image recognition. The app allows users to take a photo of their meal and receive a breakdown of macronutrients categorized by RAG/SAG levels. It's designed as both a research tool and a user-friendly prototype.

---

## Research Goal

We aim to evalate:
The accuracy of food identification from images
The reliability of macronutrient estimation (protein, fats, calories)
The effectiveness of RAG/SAG categorization for nutritional insight
The usability of the app interface across diverse users and meals

---

## App Flow

 **Welcome Scrren**  
- Brief intro and CTA to begin
 **Photo Capture Screen**  
 - Take or upload a food image
**Breakdown Screen**  
 - View estimated RAG/SAG breakdown of protein, fats, and calories



--- 

##  Developer Notes / Data Section

**2025-10-24** — Added [Nutrition5k](https://github.com/naruto36516/Nutrition5k)  
**Purpose:** Base dataset for food image recognition and nutrition  
**Notes:** This seems useful. We can use this to get a basic idea of how some people have started capturing data and saving it.

---

**2025-10-25** — Added [react-native-vision-camera](https://github.com/mrousavy/react-native-vision-camera)  
**Purpose:** A camera module with built-in pipelines for various tasks, usable on both iOS and Android  
**Notes:** This seems like a great way to collect images and feed them into our recognition pipeline. It allows users to take pictures and integrates well with our planned flow.

---

**2025-10-26** — Added [expo-image-picker](https://github.com/expo/expo/blob/main/packages/expo-image-picker/README.md)  
**Purpose:** Enables image selection from the camera roll on both Android and iOS  
**Notes:** We needed more ways to grab data beyond just live capture. This will let users upload existing images, which is great for flexibility.

---

**2025-10-26** — Added [passio-nutrition-flutter-app](https://github.com/vtrukhnov-lab/passio-nutrition-flutter-app)  
**Purpose:** A full frontend and backend app that performs similar tasks to our research goals  
**Notes:** This is a great reference for behavior and structure. It seems configurable, and we might be able to adapt parts of it to improve our own app. Honestly, this could be a viable base to study and build from.

---

**2025-10-26** — Added [Food-Image-Recognition](https://github.com/Pralhad789/Food-Image-Recognition/blob/main/README.md)  
**Purpose:** Full-stack app for food recognition and nutrition breakdown  
**Notes:** This is the best repo I’ve seen so far. It breaks down everything clearly and gives the developer full control over behavior. It could be a strong foundation to build on. If we find nothing better, this might be our starting point — and from there, we can improve or customize as needed.

---

**2025-10-28** — Started experimenting with Flutter  
**Notes:** I’ve been messing around with Flutter to see how we can personalize the apps we might use. It reminds me of Java in some ways, and honestly, I think I’ll take 5–7 days to understand it fully. Once I get a good grasp, I’ll be able to look at these repos and understand what they’re doing — and from there, implement similar logic in our project.

I’m also reviewing the CNNs used in these apps to see how we can integrate RAG/SAG without heavy coding. Most repos already output macronutrients, so I think we can wrap those outputs with RAG/SAG logic and feed that into the model. That should give us the breakdown we want without needing to retrain or rebuild from scratch.




