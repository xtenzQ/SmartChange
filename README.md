# SmartChange - JunctionX Seoul 2021

 > AI-powered web application able to track changes in urban landscape

🥉 Third winner in the **[SI Analytics](https://si-analytics.ai/eng/)** track of **[JunctionX Seoul 2021](https://junctionx-seoul-2021.oopy.io/)** Hackathon (21-23rd, May 2021)

![main page](main.png)

### Team

- 🇷🇺 **Nikita Rusetskii** (Irkutsk National Research Technical University, Russia) <a target="_blank" href="https://www.linkedin.com/in/xtenzq/" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5.svg?&style=flat-badge&logo=linkedin&logoColor=white" /></a> <a target="_blank" href="https://github.com/xtenzQ" target="_blank"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=flat-badge&logo=github&logoColor=white" /></a>
- 🇷🇺 **Konstantin Shusterzon** (Melentiev Energy Systems Institute, Russia) <a target="_blank" href="https://www.linkedin.com/in/konstantin-shusterzon-a9aa02181/" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5.svg?&style=flat-badge&logo=linkedin&logoColor=white" /></a> <a target="_blank" href="https://github.com/Exterminant" target="_blank"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=flat-badge&logo=github&logoColor=white" /></a>
- 🇷🇺 **Grunwald Lily** (Novosibirsk State University, Russia)
- 🇰🇷 **Lim Bison** (Inha University, South Korea)
- 🇰🇷 **Lee Junyong** (Inha University, South Korea)

### Technologies

- Vue.js (frontend)
- Flask (backend)
- PyTorch (machine learning library)
- Unet++ (neural network)

### How to use

1. Set up your environment. I recommend you to use anaconda for it since we're doing some machine learning:
```bash
# create conda env with Python 3.7
$ conda create -n junctionx python=3.7

# activate it
$ conda activate junctionx

# install all dependencies
$ pip install -r requirements.txt
```

2. Install Node.JS modules:
```bash
$ npm install
```

3. Run backend:
```bash
python app.py
```
It is usually run on `http://127.0.0.1:5000/`

4. Run frontend (you need second terminal):
```bash
npm run serve
```
It is usually run on `http://127.0.0.1:8080/`

5. Upload pics to neural net and get results 
   
    5.1. Go to `Upload` page 
   
    5.2. Upload two pics of the size `650x650` before and after 

    5.3. Click `Upload` button
 
    5.4. Get result and download by clicking `Download` button

### FAQ

> **What CUDA and cudNN do you use?**

I personally use CUDA 10.0 and cudNN 7.6.4

> **What Python do you use for this project?**

Python 3.7

> **How to set up conda for IntelliJ IDEA?**

`File` -> `Settings` -> `Project` -> `Project Interpreter` -> `Add` -> Pick up new conda environment or use existing

> **Why recognition is so inaccurate?**
 
We didn't have much time during hackathon, so we trained it only on 22 images.