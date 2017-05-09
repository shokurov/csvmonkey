# csvmonkey

This is a vectorized, lazy-decoding zero-copy CSV file parser. The C++ version can process ~1.7GB/sec of raw input in a single thread, the Python version is ~5x faster than `csv.reader` and ~13x faster than `csv.DictReader`, while maintaining a similarly usable interface.

Requires a CPU supporting Intel SSE4.2 and a compiler that bundles `smmintrin.h`.

It still requires a ton of work. For now it's mostly toy code