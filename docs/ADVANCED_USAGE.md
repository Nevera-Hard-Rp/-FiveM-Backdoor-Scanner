# 🔧 Advanced Usage Guide

## Table of Contents
1. [Custom Signatures](#custom-signatures)
2. [ML Detection](#ml-detection)
3. [Network Analysis](#network-analysis)
4. [Automation](#automation)
5. [Integration](#integration)

## Custom Signatures

### Creating Custom Signatures

```python
# custom_signatures.json
{
    "pattern": "TriggerServerEvent.*GiveMoney.*999999",
    "description": "Unrealistic money spawn",
    "severity": 10,
    "framework": "custom",
    "category": "exploit"
}
ML Detection
Training Custom Models
python
Copy
Edit
# ml_detector.py
import numpy as np
from sklearn.ensemble import RandomForestClassifier

class MLThreatDetector:
    def __init__(self, model_path=None):
        self.vectorizer = TfidfVectorizer(
            max_features=1000,
            ngram_range=(1, 3)
        )
        
    def train(self, training_data):
        # Training implementation
        pass
[Include all ML and advanced features from original README]
