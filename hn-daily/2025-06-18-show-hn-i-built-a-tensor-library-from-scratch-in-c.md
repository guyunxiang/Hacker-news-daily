# Show HN: I built a tensor library from scratch in C++/CUDA

**Posted by nirw4nna on 2025-06-18**

Hi HN,

Over the past few months, I’ve been building *dsc*, a tensor library from scratch in C++/CUDA. My main focus has been on getting the fundamentals right, prioritizing a clean API, simplicity, and clear observability for running small LLMs locally.

### Key Features:
- C++ core with CUDA support, written from scratch.
- A familiar, PyTorch-like Python API.
- Capable of running real models: it's complete enough to load a model like Qwen from HuggingFace and run inference on both CUDA and CPU with just a single line change [1].
- Simple, built-in observability for both Python and C++.

### Roadmap:
Next, I plan to add BF16 support. After that, I'll work on visualization tools for GPU workloads.

The project is still in early development, and I would be incredibly grateful for any feedback, code reviews, or questions from the HN community!

### GitHub Repository:
[https://github.com/nirw4nna/dsc](https://github.com/nirw4nna/dsc)

### Reference:
[Model loading example](https://github.com/nirw4nna/dsc/blob/main/examples/models/qwen2_5.py)