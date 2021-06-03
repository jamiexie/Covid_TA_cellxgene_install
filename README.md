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

## 3. Install python dependencies
pip install scanpy

pip install louvain

## 4. Install cellxgene
pip install cellxgene

## 5. Download h5ad files:
https://drive.google.com/drive/u/0/folders/1rCXJjCX5fN2_7YH2k-hmjGF7WUGEbo3Q

Save .h5ad files to your folder of choice. This folder will contain your annotations from cellxgene so make sure you know where it is!

## 6. Navigate to folder where you have saved .h5ad files and open h5ad in cellxgene
*This is the step you will do every time you want to use cellxgene*

For example, if my .h5ad is in ~/Documents/COVID_TA:

cd ~/Documents/COVID_TA

cellxgene launch [path-to-your-object/name-object.h5ad] --experimental-enable-reembedding --open

*Trick to launch h5ad if you don't know the specific path*:

Open a finder window right next to the terminal window. Select the h5ad file in finder and drag it to terminal.

Any annotations you make in cellxgene will save in a csv file in your working directory and then we can merge the annotations back into the object afterwards.

## 7. Close cellxgene when finished!
*press* ctrl+c
