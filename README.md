# test-tailwindcss
This repo is only for assessing why postcss is not installing when the usual process is followed from the tailwindcss website.<br>

## Start

Head to the Tailwindcss install page, specifically the one that includes Postcss:<br>
https://tailwindcss.com/docs/installation/using-postcss

![Tailwindcss Official install page (with Postcss)](https://github.com/ishyamo/test_tailwindcss/blob/907a1ac878c7fc48c6e85a79194b902e9cbb624c/2_tailwindcss_install_page.png "")

Following install steps:
1. Install Tailwind CSS<br>

This is the route I used on my Mac for this test:<br>
`CD Store/localdev/test-tailwindcss`

Then used:<br>
`npm install -D tailwindcss postcss autoprefixer`<br>
`npx tailwindcss init`


2. Add Tailwind to your PostCSS configuration
3. Configure your template paths
4. Add the Tailwind directives to your CSS
5. Start your build process using: npm run dev


---
Computer details: `Mac Mini running macOS Version 10.15.7 (Catalina)`  
<br>
NPM details: npm already installed via nvm.<br>  
Version info: <br> 
{  <br>
  npm: '9.8.0',  <br>
  node: '20.5.0',  <br>
  acorn: '8.10.0',  <br>
  ada: '2.5.1',  <br>
  ares: '1.19.1',  <br>
  base64: '0.5.0',  <br>
  brotli: '1.0.9',  <br>
  cjs_module_lexer: '1.2.2',  <br>
  cldr: '43.1',  <br>
  icu: '73.2',  <br>
  llhttp: '8.1.1',  <br>
  modules: '115',  <br>
  napi: '9',  <br>
  nghttp2: '1.55.1',  <br>
  nghttp3: '0.7.0',  <br>
  ngtcp2: '0.8.1',  <br>
  openssl: '3.0.9+quic',  <br>
  simdutf: '3.2.14',  <br>
  tz: '2023c',  <br>
  undici: '5.22.1',  <br>
  unicode: '15.0',  <br>
  uv: '1.46.0',  <br>
  uvwasi: '0.0.18',  <br>
  v8: '11.3.244.8-node.10',  <br>
  zlib: '1.2.13.1-motley'  <br>
}  <br>


