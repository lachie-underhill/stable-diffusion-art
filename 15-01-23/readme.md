# Week Ending Sunday 15/01/23

![first image](01.png)

![second image](02.png)

![third image](03.png)

## Details

Negative prompt remained the same throughout all steps:
`blur, haze, lowres`

### 1. Initial Gen
Model: `14e1ef5d` (dreamlike-diffusion-1.0)
Prompt: `a (matte painting) of a black hole with space dust around it, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, quantum wavetracing, imax`
Sampler: Euler a
Steps: 20
CFG: 7
Seed: 1881963886

### 2. img2img through midjrny-v4
Model: `ddc6edf2` (midjrny-v4)
Prompt: `(mdjrny-v4 style) an extremely high resolution (matte painting) of a gateway looking through to a (mountain:1.1) in space, with space dust around it, 8k, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, intricate, highly detailed, exquisite detail, quantum wavetracing, imax`
Resolution: 512x512
Sampler: DPM++ 2M Karras
Steps: 100
CFG: 7.5
Denoising: 0.7

Favourite image was cherrypicked from here

### 3. img2img back through dreamlike-diffusion
Model: `dreamlike-diffusion-1.0`
Prompt: `an extremely high resolution (matte painting) of a gateway looking through to a (mountain:1.1) in space, with space dust around it, 8k, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, intricate, highly detailed, exquisite detail, quantum wavetracing, imax`
Resolution: 1024x1024
Sampler: DPM++ 2M Karras
Steps: 100
CFG: 8.5
Denoising: 0.45

### Upscaling
Upscaler: R-ESRGAN 4x+
Resolution: 2048x2048

### Post-Processing
Noise added in paint.net


