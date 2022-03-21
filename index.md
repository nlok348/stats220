### *Assignment 1 meme* ###
![my_meme](https://user-images.githubusercontent.com/101226761/159197371-a89e3199-7d7b-4609-adaf-c7df8bc92416.png)

##### *R code used to create meme*
library(magick)

#section one

photo <- image_read("https://i.imgflip.com/4/3eqjd8.jpg") %>%
  image_scale(500)

#section two

spiderman_original <- image_blank(width = 500, height = 500, color = "#FFFFFF") %>%
  image_annotate(text = "When you thought you had an original meme", color = "#000000", size = 25, gravity = "center")

#combining sections

image_append(c(photo, spiderman_original))

### *Information about meme*
* STATS 220 Assignment 1 required an original meme
* I thought about it long and hard but I do not have a creative bone in my body
* The meme I ended up with is an adaptation of a pre-existing meme
