# docker
Docker projet for coding academy by epitech

# Vue js Project
## Installation

First, clone this repository:

# Clone this repository
git clone https://github.com/mfts/papermark.git
cd vue-project

# Build image
docker build -t vue-app . 

# Run image
docker run -it -p 5000:80 --rm --name vue-app-1 vue-app

# Open http://localhost:5000 in your browser
open http://localhost:5000