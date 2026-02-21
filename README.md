# Hello !
This is my very first time building a personal blog and the first time building on GitHub.

Nice to meet you here!

For one who wants to build a personal blog like me.

I recommend you go through the reference. Basically, I found (ref. 1) first and then just follow the instrument, haha.

The work flow to Hugo to build your personal blog are

Install Hugo, Git, Go, ... all the requirement -> Start new site -> Initial git repo -> Install theme ->
Start new post -> configure the site -> run server -> push local to remote -> build and pubsith site. 

See (ref. 2) for overview.

Here are some keypoints:

0. Know the basic of GiHub from (ref. 3)
1. Create the repository as <username>.github.io (ref.4)
2. Althrough the Hexo is mentioned in (ref. 4) and the Jekyll is recommended by GitHub (ref. 5), the file structure of Hugo is used in the (ref. 6), see (ref. 7) and (ref. 8-10) for detail.
3. So I choose Hugo too XD
4. Install Git, Go, Chocolatey, Dart Sass and Hugo, see (ref. 11-14)
  
   Where, Git-2.53.0-64-bit.ext, go1.26.0.windows-amd64.msi, Chocolatey v2.6.0, Sass 1.97.3 and hugo_extended_0.156.
   
   0_windows-amd64.zip are selected [2026/02/21]
  
   Noted, I move the "hugo.exe" to "C:\Hugo\bin" and add the "C:\hugo\bin" to PATH enviroment variable

6. Build a new site, in my case, type "hugo new site CP-Tsai-Blog" in "C:\Hugo\bin"
7. Initial git, type "git init"
8. Clone the theme you like / or subnodule the theme
   
   I choose the PaperMod for my blog, see (ref. 15)
   
   type "git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod"
   
9. Post your 1st post, for example, type "hugo new posts/mems-resoswitches-intro.md"
10. Turn on the preview function by "hugo server -D"
11. To build a automatic workflow by "git push" function, change the Setting/Build and deployment/Source from "Deploy from a branch" to "GitHub Action" first
12. Excute the uploading via

    git add .
    
    git commit -m "The action you want to record"
    
    git push -u origin cptsai.github.io
    
    *typically, "cptsai.github.io" in third line would be "main",
    however, I used the name of branch same as my website so it become irregular

Reference:
1. https://minglun-wu.medium.com/%E5%BB%BA%E7%AB%8B%E4%B8%80%E5%80%8B%E5%B1%AC%E6%96%BC%E8%87%AA%E5%B7%B1%E7%9A%84-%E7%A8%8B%E5%BC%8F-%E9%83%A8%E8%90%BD%E6%A0%BC-4d295ed96236
2. https://wellstsai.com/post/build-hugo/
3. https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#user--organization-pages
4. https://docs.github.com/en/pages/quickstart
5. https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll
6. https://minglunwu.com/
7. https://github.com/MingLunWu/MingLunWu.github.io
8. https://ithelp.ithome.com.tw/articles/10269253
9. https://raychiutw.github.io/2019/Static-Site-Generator-Comparison/
10. https://lynnblog.net/post/2023-06-17-%E6%90%AC%E5%AE%B6%E5%95%A6-%E5%BE%9Ehexo%E5%88%B0medium%E5%86%8D%E5%88%B0hugo/
11. https://gohugo.io/
12. https://zhuanlan.zhihu.com/p/105021100
13. https://hugo.makiot.com/docs/installation/windows/
14. https://devbricker.github.io/post/hugo/deploy/hugo_environment/
15. https://github.com/adityatelange/hugo-PaperMod/wiki/
