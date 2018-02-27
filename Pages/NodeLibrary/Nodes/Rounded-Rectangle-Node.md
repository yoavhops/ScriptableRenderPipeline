## Description

Generates a rounded rectangle shape based on input **UV** at the size specified by inputs **Width** and **Height**. The radius of each corner is defined by input **Radius**. The generated shape can be offset or tiled by connecting a [Tiling And Offset Node](https://github.com/Unity-Technologies/ShaderGraph/wiki/Tiling-And-Offset-Node). Note that in order to preserve the ability to offset the shape within the UV space the shape will not automatically repeat if tiled. To achieve a repeating rounded rectangle effect first connect your input through a [Fraction Node](https://github.com/Unity-Technologies/ShaderGraph/wiki/Fraction-Node).

## Ports

| Name        | Direction           | Type  | Binding | Description |
|:------------ |:-------------|:-----|:---|:---|
| UV      | Input | Vector 2 | UV | Input UV value |
| Width      | Input | Vector 1 | None | Rounded Rectangle width |
| Height      | Input | Vector 1 | None | Rounded Rectangle height |
| Radius      | Input | Vector 1 | None | Corner radius |
| Out | Output      |    Vector 1 | None | Output value |

## Shader Function

```
Radius = max(min(min(abs(Radius * 2), abs(Width)), abs(Height)), 1e-5);
float2 uv = abs(UV * 2 - 1) - float2(Width, Height) + Radius;
float d = length(max(0, uv)) / Radius;
Out = saturate((1 - d) / fwidth(d));
```