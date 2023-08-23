# test-tailwindcss
This repo is only for assessing why postcss is not installing when the usual process is followed from the tailwindcss website.<br>

## Start

Head to the Tailwindcss install page, specifically the one that includes Postcss:<br>
https://tailwindcss.com/docs/installation/using-postcss

![Tailwindcss Official install page (with Postcss)](https://github.com/ishyamo/test_tailwindcss/blob/907a1ac878c7fc48c6e85a79194b902e9cbb624c/2_tailwindcss_install_page.png "")

Following install steps:<br>
1. **Install Tailwind CSS**<br>

This is the route I used on my Mac for this test:<br>
`CD Store/localdev/test-tailwindcss`

Then used:<br>
`npm install -D tailwindcss postcss autoprefixer`<br>
`npx tailwindcss init`

Tailwind installs, but there are errors...<br>
![Install errors](https://github.com/ishyamo/test_tailwindcss/blob/77833c17f75374e738966dd0d7358f8278ec1745/3_Install_items_.png "")
<br><br>
Checking the folder shows that the post.config.js (needed for the second step in the process) is absent! :( <br>
![Folder contents - only tailwind config](https://github.com/ishyamo/test_tailwindcss/blob/5c360d02efbd99260bda9e66ca6c121985f7ff68/4_Only_tailwind_config_installed_.png "")

<br><br>
Okay, how about if we try only installing postcss in that folder: `npm install postcss`<br>

Nope, same issues and nothing installed. <br>
Right, let's run `npm audit` to see what's going on....<br><br>
The full report and just the part about Postcss were included in this repo (**Update: Now removed**)<br>

Is this typical of postcss installs? It's quite bad.<br><br>

## Update: NOW FIXED!

Please refer to: [installing tailwindcss v.3.0.15 using PostCSS doesn't work properly](https://stackoverflow.com/questions/70843629/installing-tailwindcss-v-3-0-15-using-postcss-doesnt-work-properly)
<br><br>
Running `npx tailwindcss init -p` fixed it! :) 

---
2. **Add Tailwind to your PostCSS configuration**
3. **Configure your template paths**
4. **Add the Tailwind directives to your CSS**
5. **Start your build process using: npm run dev**




