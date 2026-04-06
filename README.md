# Import GGUF Models into Ollama

---

## Overview

A `.gguf` file is a packaged model containing pretrained weights, architecture, and metadata, ready for inference.

---

## Steps

### 1. Create a `Modelfile`

```
FROM "/absolute/path/to/model.gguf"
```

---

### 2. Build the Model

Replace `<model-name>` with your desired name:

```
ollama create <model-name> -f Modelfile
```

---

### 3. Run the Model

```
ollama run <model-name>
```

---

## Notes

* The `.gguf` file path must be absolute.
* `<model-name>` is an arbitrary name used to reference the model in Ollama.
* The `.gguf` extension is the model file format, not part of the model name.
