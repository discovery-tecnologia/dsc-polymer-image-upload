# &#60;dsc-polymer-image-upload&#62;

[![Build Status](https://travis-ci.org/discovery-tecnologia/dsc-polymer-image-upload.svg?branch=master)](http://travis-ci.org/#!/discovery-tecnologia/dsc-polymer-image-upload)
![Bower version](https://img.shields.io/bower/v/dsc-polymer-image-upload.svg)
![](https://img.shields.io/pypi/l/Django.svg)

Images crop and upload.

![demo](https://raw.githubusercontent.com/discovery-tecnologia/dsc-polymer-image-upload/master/docs/img/01.jpg)
![demo](https://raw.githubusercontent.com/discovery-tecnologia/dsc-polymer-image-upload/master/docs/img/02.jpg)

Differential:

 * Easy to use
 * Fully compatible with restfull APIs (base64 encode)
 * Resize and crop image
 * JPG size optimization
 * Validate file name, width, height, aspect ratio, size and quantity of files
 * Order suport
 * Custom file name and description
 * Customizable style

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
<dsc-polymer-image-upload
    max-files="10"
    aspect-ratio="16:9"
    max-width="1920"
    max-height="1080">
</dsc-polymer-image-upload>
```

## API Reference

### Properties

| Property       | Description                                    | Default       |
|:---------------|------------------------------------------------|---------------|
| language       | Select component language ('en', 'pt' or 'es') | en            |
| max-files      | Maximum number of files                        | 5             |
| max-file-size  | Maximum size in bytes per file                 | 1024000 (1MB) |
| min-width      | Minimum image width in pixels                  | 320           |
| max-width      | Maximum image width in pixels                  | 1920          |
| min-height     | Minimum image height in pixels                 | 240           |
| max-height     | Maximum image height in pixels                 | 1080          |
| aspect-ratio   | Force aspect ratio of crop. Ex: 16:9, 4:3, 1:1, 2:3 or 0 for free | 1:1 |

### Methods

| Method           | Description                                      |
|:-----------------|--------------------------------------------------|
| **setData**()    | Set array of objects by exitent items. The format of the objects must be the same as that returned by the getData method |
| **isValid**()    | Boolean state of validation                      |
| **getData**()    | returns JSON array of object items. It is recommended to check the 'isValid' method before getting the items |

### Events

none

## Test

Check sintax and execute selenium tests.

```
$ npm test
```

## TODO
 * contrast and brightness
 * More tests
