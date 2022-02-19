# Welcome to QRCode API

A QRCode generating API to easily and quickly generate QR Codes.

## Overview

This is an api I made ages ago to generate qrcodes with a few different parameters.
Idk if I should maintain it or not.

___
## Basic Usage

### Generating the QRCode

`/qrcode` method `post`

#### Body Parameters

* `size` - The qrcode's version size.
    * Min: 3
    * Max: 45
    * Recommended: auto

* `quality` - Image quality
    * Min: 0.1
    * Max: 10
    * Recommended: 4

* `margin` - Bordering margin of the qrcode
    * Min: 0
    * Max: 200
    * Recommended: 1

* `expiry` - Image Expiry *(In seconds)*
    * Min: 10
    * Max: 300
    * Recommended: 180

* `detail` - The data you want the qrcode to hold.
    * String
    * Number
    * URL

### Retriving the Code Images

`/images/[id]` where `id` = the generated qrcode id using the `GET` method.
