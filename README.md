Mesh Quantization Example
=========================

This is a minimal example of mesh compression via vertex attribute quantization (live demo [here](https://tsherif.github.io/mesh-quantization-example/)).
It simply draws two triangles to the screen, one using standard 32-bit floats to
encode the positions, and the other with positions [quantized to 16-bit unsigned ints](https://github.com/tsherif/mesh-quantization-example/blob/gh-pages/index.html#L178) which
are then [decoded on the GPU via a single matrix multiplication](https://github.com/tsherif/mesh-quantization-example/blob/gh-pages/index.html#L59).

The technique is described in the [glTF quantized attributes extension](https://github.com/KhronosGroup/glTF/blob/master/extensions/Vendor/WEB3D_quantized_attributes/README.md) and
the original paper, [Mesh Geometry Compression for Mobile Graphics by Lee, Choe and Lee](http://cg.postech.ac.kr/research/mesh_comp_mobile/mesh_comp_mobile_conference.pdf).

