
# Pretrained StyleGAN3 for Sentinel-2 Satellite Imagery
This project utilizes [StyleGAN3](https://github.com/NVlabs/stylegan3) architecture to generate Sentinel-2 satellite imagery.

<div align="center">
  <img src="https://github.com/user-attachments/assets/72572aa6-b1d9-4ec3-b0a8-03dce7533158" alt="StyleGAN3 Model" style="max-width: 100%; height: auto;" />
</div>

## Model Details

- **Resolution:** 256x256 
- **Dataset:** Custom-made, consisting of 100k images collected from [Copernicus Browser](https://browser.dataspace.copernicus.eu/?zoom=5&lat=50.16282&lng=20.78613&demSource3D=%22MAPZEN%22&cloudCoverage=30&dateMode=SINGLE)
- **Notes:** FID = 23, trained 3.6 Mimgs, gamma = 5
- [Download Link](https://drive.google.com/file/d/15bk5vfo5AWnlt9DrNJjEjrCd5Ov19Ajz/view?usp=sharing)


## Transfer Learning

This model was developed using transfer learning techniques:

- **Base Model:** LHQ-256
- **Source:** [Awesome Pretrained StyleGAN3](https://github.com/justinpinkney/awesome-pretrained-stylegan3)

The weights from the pretrained StyleGAN3 model were used for initialization, and the model was then fine-tuned on the Sentinel-2 dataset.
