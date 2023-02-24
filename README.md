# SD_Notes
These are my Stable Diffusion notes on GitHub

#Use for refrence for github
https://docs.github.com/en/get-started/quickstart/hello-world


Open GitBash
---------------------------

$ cd ~/git_repos/AUTOMATIC1111/stable-diffusion-webui/

./webui-user.bat
$ ./webui-user.bat

(Python 3.9.13)

Type in Brower Local Host:

http://localhost:7860/

This should start Stable Diffusion.
---------------------------


Embeddings
---------------------------
Create Art From Your Face With AI For Free | Dreambooth Tutorial | Stable Diffusion Guide
https://www.youtube.com/watch?v=FaLTztGGueQ

Create Art From Your Face With AI For Free Part 2 | No Google Colab | No Code | Automatic1111 Guide
https://www.youtube.com/watch?v=P1dfwViVOIU

◆  TUTORIAL LINKS ◆ 

🖼️ | BIRME
‘Resize any image to 512x512 for free, I used Photoshop to do mine but you can use any tool that will let you set pixel size to 512x512’’
https://www.birme.net/?target_width=5...

💤 | DREAMBOOTH IN GOOGLE COLAB
‘An online workspace that will run python code which will ultimately generate your images’
https://colab.research.google.com/git...

🤗 | HUGGING FACE
‘Where you get your tokens from, these will allow access to Stable Diffusion in the Dreambooth Google Collab’
Old v1.4 Link: https://huggingface.co/CompVis/stable...
New v1.5 Link: https://huggingface.co/runwayml/stabl...

🎨 | LEXICA ART
‘Where you can see other AI art creations and the prompts used to build them up. It’s super handy if you want to start churning higher quality are out quicker’
https://lexica.art/

💬 | DISCORD
‘Pretty empty right now but the aim’s to eventually have it as a creative network where people can share insights into art and tech’
https://discord.gg/HNecqYUwZT

◆ GUIDES/ RESOURCES ◆ 

🤖 | STABLE DIFFUSION WEBUI TUTORIAL
‘Want to create AI images of anything for free? By downloading the Stable Diffusion git repository you’ll be well on your way to doing this locally from home using your own hardware. It’s a little more complicated to get up and running but you can start by following this video:’
https://youtu.be/KFdtf1JKXmQ?t=121



Stable Diffusion 1.5: Install, Comparison, Guide - Everything you need to know
https://www.youtube.com/watch?v=mUpQMx9Qimg

---------------------------------------------------------------------------------------------------------------
1/7/2023

*Wiping and re-installing the AUTOMATIC1111 directory

*SD 2.1 from huggingface

(BASH overview)
some commands:

python --version (sometimes stable diffusion webui will need newer version to run)

git status (on branch master)

git fetch (see what's changed)

git branch --all (lists all branches)

git checkout

git whatchanged or git log

(hit q to get out of all of it)

git log --oneline --graph

git clean

git clean -f (force) or -fdx (nuclear)

git reset --hard

cat webui-user.bat (see contents of file)

###SD 2.1##
Look at wikis of all of these things

download ckpts (model checkpoint files) & vae if applicable 

*LORA in AUTOMATIC1111 - a new training thing!

venv - virtual environment Python (Python dependency Hell)


-------------------------------
1/8/2023

https://rentry.org/voldy

default anime negative prompt: lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry, artist name


some test prompts:

masterpiece of male Aoyagi Hajime\(Yowamushi pedal\), 青八木　一, yowamushi pedal \(Watanabe\), medium-length  blonde hair, wearing a sohoku jersey, caustics, textile shading, high resolution illustration, blue eyes, artstation male body, in the style of wataru watanabe

Anime backgrounds embedding Trigger word:(works well with everythingv3)
anime-background-style-v2

Training hypernetworks guide:
https://rentry.org/hypernetwork4dumdums

***default webui-user.bat
********
@echo off

set PYTHON=C://Users//Owner//AppData//Local//Programs//Python//Python310//python.exe
set GIT=
set VENV_DIR=
set COMMANDLINE_ARGS= --no-half --no-half-vae

call webui.bat
********

NAI: 
Eta noise seed delta = 31337
Clip - 2

for prompts:
https://cdn.openart.ai/assets/Stable%20Diffusion%20Prompt%20Book%20From%20OpenArt%2010-28.pdf


---------
1/30/2023

Great guide on textural inversion embeddings:
https://youtu.be/2ityl_dNRNw

0.05:10, 0.02:20, 0.01:60, 0.005:200, 0.002:500, 0.001:3000, 0.0005

thorough guide on textural inversion embeddings: 
https://www.youtube.com/watch?v=dNOpWt-epdQ

Realistic skin tip from Unstable Diffusion:
Maybe lower cfg and my go to are "hasselblad photography"at the start then where the artists names go "50mm f 1.2 Canon 50"and a photographer. Maybe "detailed human skin". "CGI skin texture"in negative too

Np np. I like using Sophie Anderson and Henri Privat-Livemont (photographers)


Character Training guide from anon on UnstableDiffusion:
https://rentry.org/simplified-embed-training

---
Nai prompts:
https://novelai.io/

Multiple Characters:
https://lunarmimi.net/inspiration/novelai-anime-prompt-tips-multiple-characters/

Embeddings so far:
Aoyagi_Hajime-3400 Teshima_Junta-4200

Training rate for Anime:
0.0005:5000, 0.0001:10000 
