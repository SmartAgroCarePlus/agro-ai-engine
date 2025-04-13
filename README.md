# 🌿 Agro-AI - Engine  
**Modèle ResNet50 optimisé pour la détection de maladies des plantes avec intégration Gemini**  

---

## 📌 Description Technique  

### **Objectif**  
Classifier les images de plantes en **32 maladies courantes** (ex: mildiou, oïdium) et générer des conseils de traitement via l'API Gemini.  

### **Stack Technique**  
- **Modèle Principal** : ResNet50 fine-tuné (précision: 94.2% sur le test set)  
- **Framework** : TensorFlow/Keras  
- **API** : Flask
- **Optimisations** :  
  - Cache des prédictions (Redis)  
  - Batch processing pour haute charge  
  - Métriques Prometheus  

---

## 🚀 Démarrage Rapide  

### **Prérequis**  
- Python 3.9+  
- TensorFlow 2.10+  
- Clé API Gemini ([obtenez-la ici](https://aistudio.google.com/app/apikey))  

```bash
# 1. Cloner le dépôt  
git clone https://github.com/SmartAgroCare/agro-ai.git  

# 2. Installer les dépendances  
pip install -r requirements.txt

# 3. Lancer le serveur
python3 app.py
  # ou
python app.py
