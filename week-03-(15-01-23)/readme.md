![first image](01.png)
Prompt: `a (matte painting) of a black hole with space dust around it, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, quantum wavetracing, imax`
Model: dreamlike-diffusion-1.0 ([huggingface](https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0))
Seed: 1881963886

![second image](02.png)
Prompt: `a (matte painting) of a ((black hole)) in space, galaxy (dust), by Kilian Eng, ((retrofuturism)), space art, redshift, quantum wavetracing, imax`
Model: dreamlike-diffusion-1.0 ([huggingface](https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0))
Seed: 3203780973

![third image](03.png)
Prompt: `an extremely high resolution (matte painting) of a gateway looking through to a (mountain:1.1) in space, red haze, with space dust around it, 8k, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, intricate, highly detailed, exquisite detail, quantum wavetracing, imax`
Model: dreamlike-diffusion-1.0 ([huggingface](https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0))
Seed: 115925503

## Details

Negative prompt remained the same throughout all steps:
`blur, haze, lowres`

**1. Initial gen**
Model: dreamlike-diffusion-1.0 ([huggingface](https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0))
Sampler: Euler a
Steps: 20
CFG: 7

**2. img2img through midjrny-v4**
Model: openjourney ([huggingface](https://huggingface.co/prompthero/openjourney))
Prompt: Slight variations of initial prompt with leading `(midjrny-v4 style)` token (required by openjourney v1)
Resolution: 512x512
Sampler: `Euler a` or `DPM++ 2M Karras` (whichever one I was feeling at the time)
Steps: 100
CFG: 7.5
Denoising: 0.7

**3. img2img back through dreamlike-diffusion**
Model: dreamlike-diffusion-1.0 ([huggingface](https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0))
Resolution: 1024x1024
Sampler: DPM++ 2M Karras
Steps: 100
CFG: 8.5
Denoising: 0.45

**4. Upscaling**
Upscaler: R-ESRGAN 4x+
Final resolution: 2048x2048

**5. Post-processing**
Noise added in paint.net


