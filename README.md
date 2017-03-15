# &#60;dsc-polymer-image-upload&#62;

[![Build Status](https://travis-ci.org/discovery-tecnologia/dsc-polymer-image-upload.svg?branch=master)](http://travis-ci.org/#!/discovery-tecnologia/dsc-polymer-image-upload)
![Bower version](https://img.shields.io/bower/v/dsc-polymer-image-upload.svg)
![](https://img.shields.io/pypi/l/Django.svg)

Images crop and upload.

Custom content.

## Demo

```
$ git clone https://github.com/discovery-tecnologia/dsc-polymer-image-upload.git
$ cd dsc-polymer-image-upload
$ npm install
$ npm install -g polymer-cli
$ polymer serve
```
Open browser: http://localhost:8080/components/dsc-polymer-image-upload/demo/

## Usage

Install with:

```
$ bower i dsc-polymer-image-upload --save
```

Example usage:

```html
<dsc-polymer-image-upload>
</dsc-polymer-image-upload>
```

## API

| Property       | Description                    | Default       |
|:---------------|--------------------------------|---------------|

The content can be any HTML element or other polymer component.

| Custom property |	Description                       | Default |
|:----------------|-----------------------------------|---------|


## Test

Check sintax and execute selenium tests.

```
$ npm test
```

## TODO
 * image preview
 * contrast and brightness
 * validate aspect ratio
 * separate item in new internal polymer element
