# 📡 API Reference

## Python API

```python
class CLIScanner:
    def scan_file(self, file_path: str) -> List[Threat]:
        pass
```

## REST API

```yaml
paths:
  /scan:
    post:
      summary: Initiate resource scan
```