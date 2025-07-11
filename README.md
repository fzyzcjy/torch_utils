Utilities related to PyTorch. The code is really messy and originally written for my personal usage, but open-source here since someone wants to use it.

Currently contains:

1. **Universal Memory Profiler**: Like torch memory profiler, but can examine more low-level memory allocations, such as NCCL internal buffers. I personally used this to handle NCCL related memory issues.
2. **Python GIL Detector**: Know which thread is holding Python GIL (code is in https://github.com/fzyzcjy/py_gil_spy)
3. Merge multiple Torch Profiler traces from multiple ranks into one big trace (useful when checking cooperation between ranks).
4. Extract kernel time breakdown statistics from profiles.
