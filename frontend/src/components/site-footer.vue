<script>
export default {
  data () {
    return {
      name: 'footer',
    }
  }
}
</script>

<style lang='sass-loader'>
  $primary-color: #6C9B34;
  footer {
    height: 50px;
    max-width: 960px;
    width: 100%;
    min-width: 320px;
    display: flex;
    justify-content: space-around;
    position:absolute;
    bottom: 0;
    .footer-item {
      line-height: 50px;
      a {
        padding: 0 10px;
        color: black;
        text-decoration: none;
        &:hover {
          background-color: $primary-color;
          text-decoration: underline;
        }
      }
    }
  }
</style>

<template>
  <footer>
    <span class='footer-item'>&copy; How Renewable Is My State 2017</span>
    <span class='footer-item'><a href="#">License</a></span>
  </footer>
  <!--
  /*
  Copyright (c) 2017 How Renewable Is My State

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
  */
  -->
</template>
