## QRF: Implicit Neural Representations with Quantum Radiance Fields test
[Paper]() | [Project Page](https://yfyangd.github.io/test/) | [Vedio]()

## NeRF vs QRF
* NeRF: given a 3D position (x, y, z), viewing direction (θ, ϕ), NeRF produces static and transient colors (r, g, b) and transparency values (σ).
* QRF: architecture replaces the same task with encoding circuit, parameterized quantum circuits, and quantum activation.
<img style="float: left;" src="./image/method.png" width="70%">
<br>

## QRF Architecture
* Quantum Radiance Fields (QRF) with encoding circuits and quantum circuits produces colors (r, g, b) and transparency values (σ) given a 3D position (x, y, z) and viewing direction (θ, ϕ). Similar to the NeRF architecture, QRF enforces that the predicted σ is independent of view direction. Note that this schematic is a simplified quantum circuit with only 4 rotation gates around the z axis.
<img style="float: left;" src="./image/architecture.png" width="70%">
<br>

> **Source of Data:** World Health Organisation (**WHO**), Centers for Disease Control and Prevention (**CDC**)

> **Predict Model:** Seq2Seq (Sequence to Sequence)

> **Training Result:** Validation Score: **0.0194** MSE (**0.1394** RMSE ), **93.75%** ACC

> **Predict:**: The infection forecast for the next three days is **28348**, **33723**, **37397** (2/6,2/7,2/8). The actual number of people infected with the 2019-nCoV in the world will reach **50,000 at 02/13**


<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="466" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=b4696cc8-5dc9-11ed-b5bd-6595d9b17862"></iframe>
<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=b9f6451c-5dc9-11ed-b5bd-6595d9b17862"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=a2403828-5dc5-11ed-b5bd-6595d9b17862"></iframe>

<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
