Create a photo album folder in assets/media/albums/
Album names must be lowercase due to a Hugo bug - consider up-voting the bug with a 👍
Add images to your album folder
Paste {{< gallery album="<ALBUM-FOLDER>" >}} where you would like the gallery to appear in the page content, changing the album parameter to match the name of your album folder

How can I change the size or shape of gallery images?

Simply add resize_options when you call the gallery shortcode. This option lets you control the shape/size of gallery images using the standard Hugo resize options. For example:

{{< gallery album="<ALBUM-FOLDER>" resize_options="250x250" >}}
How can I add captions to gallery images?

Optionally, to add captions for your images, add the following instances to the end of your page’s front matter:

gallery_item:
- album: <ALBUM FOLDER>
  image: <IMAGE 1 NAME>.jpg
  caption: Write your image 1 caption here
- album: <ALBUM FOLDER>
  image: <IMAGE 2 NAME>.jpg
  caption: Write your image 2 caption here