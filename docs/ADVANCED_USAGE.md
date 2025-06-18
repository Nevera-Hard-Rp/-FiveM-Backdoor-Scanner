# 🔧 Advanced Usage Guide

## Table of Contents
1. Custom Signatures
2. ML Detection
3. Network Analysis
4. Automation
5. Integration

## Custom Signatures

```json
{
    "pattern": "TriggerServerEvent.*GiveMoney.*999999",
    "description": "Unrealistic money spawn",
    "severity": 10,
    "framework": "custom",
    "category": "exploit"
}
```

## ML Detection

Train with:

```python
from sklearn.ensemble import RandomForestClassifier

class MLThreatDetector:
    def __init__(self):
        self.vectorizer = TfidfVectorizer(max_features=1000, ngram_range=(1, 3))

    def train(self, training_data):
        pass
```