# Week Ending Sunday 08/01/23

![first image](01.png)
Prompt: `a (matte painting) of a black hole with space dust around it, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, quantum wavetracing, imax`
Seed: 822521854

![second image](02.png)
Prompt: `a (matte painting) of a black hole with space dust around it, by Kilian Eng, ((retrofuturism)), space art, redshift, quantum wavetracing, imax`
Seed: 937612730

![third image](03.png)
Prompt: `an extremely high resolution (matte painting) of a gateway looking through to a (mountain:1.1) in space, red haze, with space dust around it, 8k, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, intricate, highly detailed, exquisite detail, quantum wavetracing, imax`
Initial Seed: 115925506

## Details/Process
All prompts in this set were variations of: `a (matte painting) of a black hole with space dust around it, by Kilian Eng, (retrofuturism:1.2), space art, redshift, sci-fi,  reimagined by industrial light and magic, quantum wavetracing, imax`

Negative prompt for all: `blur, haze, lowres, low detail`

**1. Initial gen**
Model: dreamlike-diffusion-1.0
Sampler: Euler a
Steps: 20
CFG: 7

**2. Cherry-pick then img2img**
Model: dreamlike-diffusion-1.0
Resolution: 1024x1024
Sampler: Euler a
Steps: 80
CFG: 7
Denoising: 0.42

**3. Upscale**
Upscaler: R-ESRGAN 4x+
Resolution: 2x (2048x2048)

**4. Post-processing**
Noise added in paint.net


