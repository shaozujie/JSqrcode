### 说明
[JSqrcode](https://github.com/shaozujie/JSqrcode)是一个在浏览器端使用原生js生成二维码的js库，改自[Lars Jung](https://larsjung.de)的[jquery-qrcode](https://github.com/lrsjng/jquery-qrcode),在原作者的基础上去除了jquery依赖。

### 使用
[JSqrcode](https://github.com/shaozujie/JSqrcode)在`window`对象上注册了全局`qrcode`对象，使用示例如下：
```[javascript]
	qrcode(document.getElementById('container',{
    	// 渲染方式，可选`'canvas'`, `'image'` or `'div'`，默认image
    	render: 'canvas',

    	// version range somewhere in 1 .. 40
    	minVersion: 1,
    	maxVersion: 40,

    	// error correction level: `'L'`, `'M'`, `'Q'` or `'H'`
    	ecLevel: 'L',

    	// offset in pixel if drawn onto existing canvas
    	left: 0,
    	top: 0,

    	// size in pixel
    	size: 200,

    	// code color or image element
    	fill: '#000',

    	// background color or image element, `null` for transparent background
    	background: null,

    	// content
    	text: 'no text',

    	// corner radius relative to module width: 0.0 .. 0.5
    	radius: 0,

    	// quiet zone in modules
    	quiet: 0,

    	// modes
    	// 0: normal
    	// 1: label strip
    	// 2: label box
    	// 3: image strip
    	// 4: image box
    	mode: 0,

		// label大小比例和相对位置
    	mSize: 0.1,
    	mPosX: 0.5,
    	mPosY: 0.5,

    	label: 'no label',
    	fontname: 'sans',
    	fontcolor: '#000',

    	image: null
    }))
```






### 注：以下为[jquery-qrcode](https://github.com/lrsjng/jquery-qrcode)原说明

## jQuery.qrcode

[![license][license-img]][github] [![web][web-img]][web] [![github][github-img]][github] [![bower][bower-img]][github]

jQuery plugin to dynamically generate QR codes. Uses [QR Code Generator][qrcode] (MIT).


## License
The MIT License (MIT)

Copyright (c) 2016 Lars Jung (https://larsjung.de)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


[web]: https://larsjung.de/qrcode/
[github]: https://github.com/lrsjng/jquery-qrcode

[license-img]: https://img.shields.io/badge/license-MIT-a0a060.svg?style=flat-square
[web-img]: https://img.shields.io/badge/web-larsjung.de/qrcode-a0a060.svg?style=flat-square
[github-img]: https://img.shields.io/badge/github-lrsjng/jquery--qrcode-a0a060.svg?style=flat-square
[bower-img]: https://img.shields.io/badge/bower-lrsjng/jquery--qrcode-a0a060.svg?style=flat-square

[qrcode]: https://github.com/kazuhikoarase/qrcode-generator
