---
title: "Smart Glasses"
collection: portfolio
order: 4
header:
  teaser: Smart_Glasses.png
  teaser_alt: "Assistive smart glasses prototype"
lead_image: /images/Smart_Glasses.png
lead_image_alt: "Tesseract, OpenCV and eSpeak logos connected by arrows"
lead_image_caption: "The software pipeline. OpenCV prepares the image, Tesseract extracts the text, and eSpeak speaks it."
summary: "Glasses with a Raspberry Pi camera that read printed text aloud and recognize familiar faces, built to help visually impaired people."
links:
  - label: Code
    url: https://github.com/virajparimi/Smart_Glasses
    icon: code
---

Braille needs special equipment and translated copies, so much printed text stays out of reach for visually impaired readers. We built a wearable prototype in which a Raspberry Pi camera mounted on glasses photographs a page. OpenCV finds the page and cleans up the image, Tesseract reads the text, and eSpeak reads it aloud, all without an Internet connection. The glasses also recognize familiar faces with OpenCV's LBPH recognizer and can learn new ones. The prototype was **selected for the Delhi Mini Maker Faire**.
