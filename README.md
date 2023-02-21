## First, create a virtual enviroment, activate the enviroment.
`python -m venv env`

`.\env\Script\activate`

then install this package-

`pip install tensorflow matplotlib opencv`

## This is our [dataset link](https://www.kaggle.com/datasets/salviohexia/isic-2019-skin-lesion-images-for-classification)

`Downlaod the dataset and rename the dataset directory as "archive"`

--------------------------

## Then, I run the `01. Data Preprocessing.ipynb` notebook, first I saw the total numvber of images of each subfolders are-

- In directory 'AK', there are 867 image items.
- In directory 'BCC', there are 3323 image items.
- In directory 'BKL', there are 2624 image items.
- In directory 'DF', there are 239 image items.
- In directory 'MEL', there are 4522 image items.
- In directory 'NV', there are 12875 image items.
- In directory 'SCC', there are 628 image items.
- In directory 'VASC', there are 253 image items.

*Total number of Images in the 'archive' directory folder are 25331 image items*

and then I randomly selected 750 images from each subfolders and remove the skin hair of that images. 

- In directory 'AK', there are 750 image items.
- In directory 'BCC', there are 750 image items.
- In directory 'BKL', there are 750 image items.
- In directory 'DF', there are 239 image items.
- In directory 'MEL', there are 750 image items.
- In directory 'NV', there are 750 image items.
- In directory 'SCC', there are 628 image items.
- In directory 'VASC', there are 253 image items.


## after that I run the `02. Image Augmentation.ipynb` notebook, From notebook 01, I found that every folder size is not same, Thats why data augmentation is needed. Then, I choose those subfolder are less than 750 images. then randomly perform some image augmenation.

- In directory 'AK', there are 750 image items.
- In directory 'BCC', there are 750 image items.
- In directory 'BKL', there are 750 image items.
- In directory 'DF', there are 750 image items.
- In directory 'MEL', there are 750 image items.
- In directory 'NV', there are 750 image items.
- In directory 'SCC', there are 750 image items.
- In directory 'VASC', there are 750 image items.

*Total number of Images in the 'archive' directory folder are 6000 image items*

## then thirdly I run the `03. Split Data.ipynb` notebook.

I split the data into three parts.

`"Test": total 15% data`
- Subdirectory Model Data\Test\AK contains 112 image(s).
- Subdirectory Model Data\Test\BCC contains 112 image(s).
- Subdirectory Model Data\Test\BKL contains 112 image(s).
- Subdirectory Model Data\Test\DF contains 112 image(s).
- Subdirectory Model Data\Test\MEL contains 112 image(s).
- Subdirectory Model Data\Test\NV contains 112 image(s).
- Subdirectory Model Data\Test\SCC contains 112 image(s).
- Subdirectory Model Data\Test\VASC contains 112 image(s).

`"Train": total 70% data`
- Subdirectory Model Data\Train\AK contains 525 image(s).
- Subdirectory Model Data\Train\BCC contains 525 image(s).
- Subdirectory Model Data\Train\BKL contains 525 image(s).
- Subdirectory Model Data\Train\DF contains 525 image(s).
- Subdirectory Model Data\Train\MEL contains 525 image(s).
- Subdirectory Model Data\Train\NV contains 525 image(s).
- Subdirectory Model Data\Train\SCC contains 525 image(s).
- Subdirectory Model Data\Train\VASC contains 525 image(s).

`"Validation": total 15% data`
- Subdirectory Model Data\Validation\AK contains 113 image(s).
- Subdirectory Model Data\Validation\BCC contains 113 image(s).
- Subdirectory Model Data\Validation\BKL contains 113 image(s).
- Subdirectory Model Data\Validation\DF contains 113 image(s).
- Subdirectory Model Data\Validation\MEL contains 113 image(s).
- Subdirectory Model Data\Validation\NV contains 113 image(s).
- Subdirectory Model Data\Validation\SCC contains 113 image(s).
- Subdirectory Model Data\Validation\VASC contains 113 image(s).


--------------------------

## I created many directories with the subdirectories but finally I got `Model Data` folder.

## In "Model Data folder"
- In directory 'AK', there are 750 image items.
- In directory 'BCC', there are 750 image items.
- In directory 'BKL', there are 750 image items.
- In directory 'DF', there are 750 image items.
- In directory 'MEL', there are 750 image items.
- In directory 'NV', there are 750 image items.
- In directory 'SCC', there are 750 image items.
- In directory 'VASC', there are 750 image items.


--------------------------


## Finally, I run the `04. Custom CNN Model.ipynb` notebook

--------------------------