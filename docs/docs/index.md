# Welcome to QRCode API

A QRCode generating API to easily and quickly generate QR Codes.

## Overview

a

___
## Basic Usage

### Generating the Codes

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

`/images/[id]` where `id` = the generated qrcode id
