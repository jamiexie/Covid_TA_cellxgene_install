# Covid_TA_cellxgene_install
Installation instructions for COVID TA project
Modeling after Angela Pisco's tutorial: https://github.com/czbiohub/cellxgene-training
Cellxgene documentation for reference:
https://chanzuckerberg.github.io/cellxgene/posts/install

*Make sure you have Google Chrome working on your computer*

Assuming you're working from a clean MacOS environment:
## 1. Install Anaconda
Download: https://www.anaconda.com/products/individual
Installation instructions: https://docs.anaconda.com/anaconda/install/mac-os/

## 2. Open terminal
Spotlight search (command+space bar): terminal

## 3. Create a conda environment for cellxgene
conda create -n cellxgene python=3.8.2

## 4. Activate conda environment
conda activate cellxgene

## 5. Install python dependencies
pip install scanpy
pip install louvain

## 6. Install cellxgene
pip install cellxgene

## 7. Download h5ad files (using colon/ileum as example):
https://drive.google.com/drive/u/0/folders/1rCXJjCX5fN2_7YH2k-hmjGF7WUGEbo3Q
Save .h5ad files to your folder of choice.

## 8. Open h5ad in cellxgene
cellxgene launch [path-to-your-object/name-object.h5ad] --experimental-annotations-ontology --experimental-enable-reembedding --open

*Trick to launch h5ad if you don't know the specific path*:
Open a finder window right next to the terminal window. Select the h5ad file in finder and drag it to terminal.

Any annotations you make in cellxgene will save in a csv file in your working directory and then we can merge the annotations back into the object afterwards.
