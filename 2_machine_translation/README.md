# Introduction
The translation from Arabic and Spanish files to English using Google API, MS Azure, Deep learning, DeepL, and Transformers, and evaluates translation quality using BLEU, METEOR, and BERT scores matrices.
This repository provides scripts for translating Arabic and Spanish files to English quality checks.
# Translation
The following translation services were used:
Google API:
Use Google Translate API to translate text.
Azure Translator:
Use Azure Translator API to translate text.
Deep Learning Translator (GoogleTranslator):
Use Deep Learning Translator API to translate text.
DeepL Translator:
Use DeepL API to translate text.
Transformers:
Use Hugging Face Transformers models (Helsinki-NLP) for translation.
# Quality Evaluation
The quality check was between the English-translated text with the Native speaker generated dataset using:
BLEU.
METEOR.
BERT scores.
# Prerequisites
General:
import pandas as pd
import os

Google API:
!pip install google-cloud-translate pandas
from google.cloud import translate_v2 as translate
Azure Translator:
!pip install deep-translator pandas
Deep Learning Translator:
from deep_translator import GoogleTranslator
!pip install deep-translator pandas
Transformers:
!pip install transformers pandas torch
!pip install sentencepiece
!pip install transformers pandas torch sentencepiece
# Define model names for translations
arabic_to_english_model = 'Helsinki-NLP/opus-mt-ar-en'
spanish_to_english_model = 'Helsinki-NLP/opus-mt-es-en'






