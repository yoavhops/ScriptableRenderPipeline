## Description

When using `CodeFunctionNode` you are able to define [Ports](https://github.com/Unity-Technologies/ShaderGraph/wiki/Port) with any **Bindings** that available in [Shader Graph](https://github.com/Unity-Technologies/ShaderGraph/wiki/Shader-Graph). For a full list of available **Bindings** see [Port Bindings](https://github.com/Unity-Technologies/ShaderGraph/wiki/Port-Bindings). When using `CodeFunctionNode` **Bindings** are defined using [SlotAttribute](https://github.com/Unity-Technologies/ShaderGraph/wiki/SlotAttribute).

For more information on how to create [Nodes](https://github.com/Unity-Technologies/ShaderGraph/wiki/Node) using `CodeFunctionNode` see [Custom Nodes with CodeFunctionNode](https://github.com/Unity-Technologies/ShaderGraph/wiki/Custom-Nodes-With-CodeFunctionNode).

Below is a full list including the [Port Bindings](https://github.com/Unity-Technologies/ShaderGraph/wiki/Port-Bindings) they map to.

## Bindings

| SlotAttribute Binding | Port Binding |
|:-------------|:------|
| ObjectSpaceNormal | Normal (in object space) |
| ObjectSpaceTangent | Tangent (in object space) |
| ObjectSpaceBitangent | Bitangent (in object space) |
| ObjectSpacePosition | Position (in object space) |
| ViewSpaceNormal | Normal (in view space) |
| ViewSpaceTangent | Tangent (in view space) |
| ViewSpaceBitangent | Bitangent (in view space) |
| ViewSpacePosition | Position (in view space) |
| WorldSpaceNormal | Normal (in world space) |
| WorldSpaceTangent | Tangent (in world space) |
| WorldSpaceBitangent | Bitangent (in world space) |
| WorldSpacePosition | Position (in world space) |
| TangentSpaceNormal | Normal (in tangent space) |
| TangentSpaceTangent | Tangent (in tangent space) |
| TangentSpaceBitangent | Bitangent (in tangent space) |
| TangentSpacePosition | Position (in tangent space) |
| MeshUV0 | UV (channel 0) |
| MeshUV1 | UV (channel 1) |
| MeshUV2 | UV (channel 2) |
| MeshUV3 | UV (channel 3) |
| ScreenPosition | Screen Position (Default mode) |
| ObjectSpaceViewDirection | View Direction (in object space) |
| ViewSpaceViewDirection | View Direction (in view space) |
| WorldSpaceViewDirection | View Direction (in world space) |
| TangentSpaceViewDirection | View Direction (in tangent space) |
| VertexColor | Vertex Color |