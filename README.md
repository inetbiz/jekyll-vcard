# Jekyll vCard 3.0 Generator
This Jekyll plugin fetches images from the web and renders their corresponding base64 codes.

For example, a 1×1 clear PNG would become:

<img src="data:image;base64, iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAAAXNSR0IArs4c6QAAAAxJREFUCNdj+P//PwAF/gL+3MxZ5wAAAABJRU5ErkJggg== " />
Be sure to know your reasons when using this plugin.

## Installation
**ADD** 

cd ${PATH_TO_JEKYLL_SITE}
echo "gem 'jekyll_image_encode'" >> Gemfile
bundle
echo "require 'jekyll_image_encode'" >> _plugins/ext.rb
Alternatively you may accomplish the same without echo and bundle:

Install the plugin by running gem install jekyll_image_encode
Add the line require 'jekyll_image_encode' to _plugins/ext.rb
Usage
In the source attribute of an HTML img element, call the base64-tag providing the image URL as the only parameter:

<img src="{% base64 http://example.org/image.png %}" />
This works for both remote (http://…) and local urls within your jekyll project.

License
Jekyll Image Embed is released under the MIT License.
