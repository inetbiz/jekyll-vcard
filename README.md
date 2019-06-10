# Jekyll vCard 3.0 Generator
This Jekyll plugin fetches images from the web and renders their corresponding base64 encoding.

For example, a logo would become:

```liquid
PHOTO;ENCODING=b;TYPE=JPEG:{% base64 http://legaldemo.strikehawk.com/assets/images/balance-scale-solid.jpg %}`
```

## Installation
**ADD** `jekyll_image_encode.rb` to your **_plugins** folder.

## Modify Gemfile
Add mimemagic gem to your Gemfile
```ruby
source 'https://rubygems.org'

gem "jekyll", group: :jekyll_plugins

group :jekyll_plugins do
  ~~~
end

  gem 'mimemagic', '~> 0.3.3'
```

## Modify _config.yml
Add the following to your config file:
```# The location
tel: (352) 123-1234
logo: balance-scale-solid.png
email: sales@services.strikehawk.com
addr: 1720 NW 38TH AVE.\n#57
city: Ocala
state: FL
zip: 34482
country: United States
lat: 29.205120
long: -82.318940
timezone: America/New_York
lang: en-US
```
## Add the liquid page template for vcard
Add the vcard template to your **pages** folder
