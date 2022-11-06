## QRF: Implicit Neural Representations with Quantum Radiance Fields test
[Paper]() | [Project Page](https://yfyangd.github.io/QRF/) | [Vedio]() | [Code]()

## NeRF vs QRF
* NeRF: given a 3D position (x, y, z), viewing direction (θ, ϕ), NeRF produces static and transient colors (r, g, b) and transparency values (σ).
* QRF: architecture replaces the same task with encoding circuit, parameterized quantum circuits, and quantum activation.

<img style="float: left;" src="./image/method.png" width="100%">


## QRF Architecture
* Quantum Radiance Fields (QRF) with encoding circuits and quantum circuits produces colors (r, g, b) and transparency values (σ) given a 3D position (x, y, z) and viewing direction (θ, ϕ). Similar to the NeRF architecture, QRF enforces that the predicted σ is independent of view direction. Note that this schematic is a simplified quantum circuit with only 4 rotation gates around the z axis.

<img style="float: left;" src="./image/architecture.png" width="100%">


## Comparison
* Volume rendering of Chair, Ship, and Hotdog with training 100k iterations. Compared with NeRF, QRF has faster convergence, higher rendering efficiency, and higher rendering quality under the quantum integration.

<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="466" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=b4696cc8-5dc9-11ed-b5bd-6595d9b17862"></iframe>
<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=b9f6451c-5dc9-11ed-b5bd-6595d9b17862"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=a2403828-5dc5-11ed-b5bd-6595d9b17862"></iframe>

## Results on real-world captured data
<br>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>
<iframe frameborder="0" class="juxtapose" width="40%" height="264" src="https://www.youtube.com/embed/80vbhPJXSCM"></iframe>

## Results on custom casual capturing
* Volume rendering: Pine Tree in front of my home
* Training: 4k iterations
* Camera position from [COLMAP](https://colmap.github.io/)


<img style="float: left;" src="https://drive.google.com/uc?export=view&id=14Rl5hms9deggISA9TXJtLR2JJN7GmEcA" width="50%" title="NeRF">
<img style="float: left;" src="https://drive.google.com/uc?export=view&id=1tXFLgWGWXWS7DucmBS6nvyuT-8T0h_jw" width="50%" title="QRF">


