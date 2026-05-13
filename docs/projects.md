---
layout: page
title: /projects
permalink: /projects/
---
# Projects
-----
<div class="split-container" markdown=1>
<img src="/assets/CTHULHU.png" alt="CTHULHU Project Board" class="image">
<div class="text" markdown=1>

# <u>Cancer-Targeting Hyperspectral Ultraprecise LASER Handling Unit (CTHULHU)</u>
***Second Place EECE Capstone Winner***
A 6-person capstone project created for Northeastern's Spring Lab and Embedded Systems to create a data pipeline that quickly processes 32-channels of photometric data from a brain cancer-probing LASER while simultaneously controlling it. The system uses an AUBoard-15P to process the channels from a custom oscilloscope board connected via LVDS connection, which it sends to a host PC over a PCIe DMA.

For this project, I designed and programmed a high-level C++ firmware library to abstract the AXI4-S data stream and ADC's SPI initialization sequence so it could be used by Northeastern’s Embedded Systems Lab. I also implemented a PCIe interface on the FPGA that processes frames of 32 channels of ADC data from a custom oscilloscope board and sends them to the host PC through AXI4-Stream protocol and receives control data from the host PC for a piezo motor-controlled LASER.

<a href="/assets/C02 Final Report - CTHULHU.pdf" target="_blank">Download - CTHULHU Final Report</a>
</div>
</div>

<div class="split-container-right" markdown=1>
<img src="/assets/FPGAAudioMixer.png" alt="FPGA Audio Mixer Block Diagram" class="image">
<div class="text" markdown=1>

# <u>FPGA-Based Audio Mixer</u>
A hardware-based audio mixer built with an AUP-ZU3 Zynq FPGA. The Zynq processor runs python code to pack 8 stem files in wave format into a single AXI-Stream of audio samples. That is streamed to the fabric, where a module programmed using Vitis HLS mixes the stem files together based on which on-board switches are on and applies audio compression and limiters to ensure there isn't distoration that occured during mixing. The final audio stream is outputted to the on-board audio codec using an I2S transmitter.
Example with one stem streamed through the fabric:
<audio src="/assets/FPGA_mix_1.mp3" controls>
    Your browser does not support audio playback
</audio>
Example with two stems mixed together in-fabric:
<audio src="/assets/FPGA_mix_2.mp3" controls>
    Your browser does not support audio playback
</audio>
<small>Stems obtained from Jamie Paige under Creative Commons BY-NC-SA license</small>
</div>
</div>

<div class="split-container" markdown=1>
<video controls>
    <source src="/assets/StarshipTheremin.mp4" type="video/mp4">
    Your browser does not support video playback
</video>
<div class="text" markdown=1>

# <u>Starship Theremin</u>
A theremin instrument that is internally powered, has a built-in speaker for use anywhere, and changes lights in a constellation based on the theremin's volume. Programmed in C++ on an Arduino Uno with a modified theremin PCB.
</div>
</div>
