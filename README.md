## Overview
Extracting more information from ID-card
1. Extracting text using ocr
2. Extracting human photo using CascadeClassifier

## Motivation
- While using some e-learning for a climbing certificate, I used my college ID which takes 2 to 3 days minimum to validate. 
- Then I started thinking about how to make it automated so I researched and change my imagination into working model.

## Technical Aspect
This project is divided into two part:
1. Extracting text using tesseract-ocr-ind package. While Tesseract is known as one of the most accurate free OCR engines available today, it has numerous advantages that dramatically affect its performance; its ability to correctly recognize characters in a scan or image.
2. Extracting human photo using CascadeClassifier and crop it, it is very fast at computing Haar-like features due to the use of integral images


## To Do
1. Working with how to make sure given image is not rotated.
2. Add a better accuracy to image croping.


## Technologies Used
 1. Open CV2
 2. tesseract-ocr-ind
 3. CascadeClassifier
 4. Basic required pakages
