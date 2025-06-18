# 📡 API Reference

## Python API

### Scanner Class

```python
class CLIScanner:
    """Main scanner class for FiveM resources"""
    
    def scan_file(self, file_path: str) -> List[Threat]:
        """
        Scan a single file for threats
        
        Args:
            file_path: Path to file to scan
            
        Returns:
            List of Threat objects found
        """
REST API
Endpoints
yaml
Copy
Edit
openapi: 3.0.0
info:
  title: FiveM Scanner API
  version: 2.0.0

paths:
  /scan:
    post:
      summary: Initiate resource scan
[Include all API documentation]
