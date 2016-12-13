# Designkit Messages

## Install

```bash
npm i designkit-messages
```

## Usage

```html
<span class="message">
  <svg class="message-icon" xmlns="http://www.w3.org/2000/svg" width="8" height="10" viewBox="0 0 8 10">
    <path fill="#FFF" fill-rule="evenodd" d="M8 9.333c0 .334-.333.667-.667.667H.667C.333 10 0 9.667 0 9.333V4.667C0 4.333.333 4 .667 4h.666V2.667C1.333 1.2 2.533 0 4 0c1.467 0 2.667 1.2 2.667 2.667V4h.666c.334 0 .667.333.667.667v4.666zm-8-4h8V6H0v-.667zM5.333 4V2.73c0-.775-.533-1.397-1.33-1.397-.803 0-1.33.622-1.33 1.397V4h2.66z"/>
  </svg>
  Basic Default Message
  <span class="message-extend">
    <svg class="message-extend-icon" xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 14 14">
      <path fill="#FFF" fill-rule="evenodd" d="M6.75.855c1.575 0 3.06.63 4.185 1.71 1.125 1.125 1.71 2.61 1.71 4.185 0 1.575-.63 3.06-1.71 4.185-1.125 1.125-2.61 1.71-4.185 1.71-1.575 0-3.06-.63-4.185-1.71C1.44 9.855.855 8.325.855 6.75c0-1.575.63-3.06 1.71-4.185C3.645 1.44 5.175.855 6.75.855zm0-.855C3.015 0 0 3.015 0 6.75s3.015 6.75 6.75 6.75 6.75-3.015 6.75-6.75S10.485 0 6.75 0zm0 2.52c-.72 0-1.26.585-1.26 1.26s.585 1.26 1.26 1.26 1.26-.585 1.26-1.26-.54-1.26-1.26-1.26zm0 3.375h-.855c-.45 0-.855.36-.855.855 0 .45.36.855.855.855v2.52c0 .45.36.855.855.855.45 0 .855-.36.855-.855V6.75c0-.45-.405-.855-.855-.855z"/>
    </svg>
  </span>
</span>
```

## The CSS

```css
/*
//
// designkit-messages
// --------------------------------------------------
*/
.message {
  position: relative;
  bottom: 3px;
  display: inline-block;
  height: 22px;
  padding: 0 8px 0 25px;
  margin-top: 4px;
  margin-left: 4px;
  overflow: hidden;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 11px;
  font-weight: bold;
  line-height: 22px;
  color: #89887a;
  cursor: pointer;
  cursor: hand;
  background-color: #FFF7E5;
  border-radius: 2px;
  -ms-flex-item-align: center;
      -ms-grid-row-align: center;
      align-self: center;
}

.message .message-icon path,
.message .message-extend-icon path {
  fill: currentColor;
}

.message .message-icon {
  position: absolute;
  top: 6px;
  left: 8px;
}

.message .message-extend {
  position: relative;
  display: block;
  float: right;
  width: 0;
  height: 22px;
  margin: 0 -8px 0 8px;
  white-space: nowrap;
  background-color: #ffefcc;
  border-radius: inherit;
  border-top-left-radius: 0;
  border-bottom-left-radius: 0;
  opacity: 0;
  -webkit-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
}

.message .message-extend .message-extend-icon {
  position: absolute;
  top: 4px;
  left: 5px;
}

.message:hover .message-extend {
  width: 24px;
  opacity: 1;
}

.message.message-dark {
  position: relative;
  color: #fff;
  cursor: pointer;
  cursor: hand;
  background-color: #353B41;
}

.message.message-dark .message-icon path,
.message.message-dark .message-extend-icon path {
  fill: currentColor;
}

.message.message-dark .message-extend {
  background-color: #57626C;
}
```

## Author

Jason Melgoza

## License

The MIT License (MIT)

Copyright (c) 2016 RightScale

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
