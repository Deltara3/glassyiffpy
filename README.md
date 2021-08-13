# glassyiffpy
## _simple code for fetching yiff images from yiff-party_

by [Glass-Paramedic](https://www.reddit.com/user/Glass-Paramedic)



##Features

- Return random yiff image
- Return newest yiff images in any category
- Iterate over submissions live as they are uploaded (new images are uploaded roughly every five minutes)


#Usage

>pip install glassyifpy


```python

horni.help() # prints a brief overview like this

from glassyifpy import horni


print(horni.randomIMG())
# result will be a random image url


print(horni.newsest("gay"))
# result will be the newsest image url in the 'gay' category.

#You can input any of the six categories or 'main' for the main page which icludes all categories
#(gay/lesbian/straight/animated/anthro/feral/main)


for image in horni.yiff(50,"anthro"):
  print(image)

#>this will return a list of 50 images in the anthro category


for image in horni.stream("main"):
  print(image)

#>This loop will run forever, printing out the images urls as they are uploaded to the site.

```
