<div align="center">
  <br>

  <h1>๋์ GitBlog </h1>

</div>

<p align="center">
 
  <a href="http://badge.fury.io/rb/jekyll-theme-yat">
    <img src="https://badge.fury.io/rb/jekyll-theme-yat.svg"
      alt="Gem Version" />
  </a>

  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-brightgreen.svg"
      alt="License: MIT" />
  </a>

  <a href="https://liberapay.com/jeffreytse">
    <img src="http://img.shields.io/liberapay/goal/jeffreytse.svg?logo=liberapay"
      alt="Donate (Liberapay)" />
  </a>

  <a href="https://patreon.com/jeffreytse">
    <img src="https://img.shields.io/badge/support-patreon-F96854.svg?style=flat-square"
      alt="Donate (Patreon)" />
  </a>

  <a href="https://ko-fi.com/jeffreytse">
  <img height="20" src="https://www.ko-fi.com/img/githubbutton_sm.svg"
  alt="Donate (Ko-fi)" />
  </a>
</p>

<br>


<h3 align="center">๐ Night Mode</h3>

<p align="center">

  <img src="https://user-images.githubusercontent.com/9413601/94983351-760f6e00-0574-11eb-9494-5303ad6228dc.gif" alt="demo-screenshot" width="780px"/>

</p>

## โจ Git ์์ํ๊ธฐ
  
  - Git ๋ก์ปฌ ์ ์ฅ์ ์์ฑ
  ```
  user $ git init
  ```
  &#8594; ํ์ฌ ์์์ค์ธ ๋๋ ํ ๋ฆฌ๋ฅผ git ์ ์ฅ์๋ก ์ง์ ํ๊ธฐ
  
  - Git์ ๋ณ๊ฒฝ์ฌํญ ๋ฐ์ํ๊ธฐ
  ```
  user $ git status
  ```
  &#8594; ํ์ฌ Git ์ํ ํ์ธ
  
  ```
  user $ git add example.py
  ```
  &#8594;example.py๋ฅผ ์์ฑ/์์ ํ๊ณ , ์ด๋ฅผ Commit์ ๋ฐ์ํ๊ณ  ์ถ์ ๊ฒฝ์ฐ
  
  ```
  user $ git commit -m "add example.py"
  ```
  &#8594; ๋ณ๊ฒฝ์ฌํญ์ด ๋ฐ์๋ new commit ์์ฑ
  
  ```
  user $ git log
  ```
  &#8594; commit ๊ธฐ๋ก ํ์ธํ๊ธฐ (Author, Commitor, Date, ...)
  
  - Git Branch ์์ฑ
  ```
  user $ git branch <branch_name>
  ```
  &#8594; git branch๋ฅผ ์์ฑ
  
  ```
  user $ git checkout <branch_name>
  ```
  &#8594; ํ์ฌ ์์์ค์ธ branch๋ฅผ ์ ํ
  
  ```
  user $ git merge <branch_name>
  ```
  &#8594; ํ์ฌ ์์์ค์ธ branch๋ฅผ ์ํ๋ branch์ ๋ณํฉ
  
  ```
  user $ git branch -d <branch_name>
  ```
  &#8594; branch๋ฅผ ์ญ์ 

## ๐ ๏ธ  Github Repo๋ฅผ Webpage๋ก ๋ง๋ค๊ธฐ
  - Github Page ์์ํ๊ธฐ
  1. Repository ์์ฑ<br>
    Github์์ <username>.github.io ์ด๋ฆ์ Repo ์์ฑ<br>
  2. Local-Remote Repository ์ฐ๋<br>
    ์์ฑํ Repo์์ Remote Repository์ ์ฃผ์ ๋ณต์ฌ<br>
    ```
    git clone <repo_name> <path>
    ```<br>
    &#8594; git clone์ผ๋ก ํด๋ก ํ๊ธฐ<br>
  3.์์ ๋ฌธ์ ์์ฑ<br>
    ์์ ํ์ผ(index.html) ์์ฑ<br>
  4. git commit ๋จ๊ธฐ๊ธฐ<br>
    ```
    git status
    git add
    ```<br>
    &#8594; git status๋ก ํ์ฌ ์ํ ํ์ธ ํ git add๋ก ๋ณ๊ฒฝํ์ผ ์ถ๊ฐ<br>
    ```
    git commit -m "msg"
    ```<br>
    &#8594; ์ปค๋ฐ ๋จ๊ธฐ๊ธฐ<br>
  5. git push๋ก ์๊ฒฉ ์ ์ฅ์์ ๋ฐ์ํ๊ธฐ<br>
    ```
    git branch -M main
    ```<br>
    &#8594; ํ์ฌ branch์ ์ด๋ฆ์ main์ผ๋ก ๋ณ๊ฒฝ<br>
    ```
    git status
    git add index.html
    ```<br>
    &#8594; git status๋ก ํ์ฌ ์ํ ํ์ธ ํ git add๋ก ๋ณ๊ฒฝํ์ผ ์ถ๊ฐ<br>
    ```
    git push origin main
    ```<br>
    &#8594; git push๋ฅผ ํตํด ์๊ฒฉ์ ์ฅ์์ ๋ฐ์<br>
    &#8594; Password์ PAT(Personal Access Token)์ ์๋ ฅํ์ฌ git pushํ๊ธฐ<br>
  6. Github Page ์ค์  ํ์ธ<br>
    &#8594; Repository Settings > Pages > ์ค๊ฐ์ ์๋ ์ฃผ์(username.github.io) ์ ์<br>
    &#8594; ์ด์ ์ ์๋ ฅํ HTML ๋ฌธ์๊ฐ ์ ๋จ๋ฉด ์ฑ๊ณต<br>
  
## โ๏ธ Build Jekyll Project
  &#8594; Local Repository์์ Jeykll ์์ ํ, ์๊ฒฉ ์ ์ฅ์์ ์ด๋ฅผ ๋ฐ์ํ๊ธฐ
  - Jekyll ์ค์น
  ```
  jekyll -v
  ```
  &#8594; Jekyll์ด ์ค์น๋์ด์๋์ง ํ์ธ
  - Jekyll ์์ํ๊ธฐ
  ```
  jekyll new . --force
  ```
   &#8594; ํ์ฌ ๋๋ ํ ๋ฆฌ(.).์ Jekyll ์ค์น
  ```
  bundle exec jekyll serve
  ```
  &#8594; (bundle exec) jekyll serve ์คํ ํ, localhost:4000 ์ ์
  &#8594; ๊ธฐ๋ณธ ํ๋ง์ Jekyll ์ฌ์ดํธ๊ฐ ์์ฑ๋จ์ ํ์ธ
  - _config.yml
  ๋๋ถ๋ถ์ ๋ธ๋ก๊ทธ ์์ฑ์ ๊ด๋ฆฌํ๋ ํ์ผ<br>
  ์ํ๋ ๋๋ก ์์ ํ ํ (bundle exec) jekyll serve๋ฅผ ์คํ
  - commit ๋จ๊ธฐ๊ธฐ
  ```
  git rm index.html
  git add *
  ```
  &#8594; git rm/git add๋ฅผ ํตํด ๋ณ๊ฒฝ์ฌํญ์ ๋ฐ์ํ  ํ์ผ๋ค ์ง์ 
  ```
  git commit -m "add: jekyll on repository"
  ```
  &#8594; ๋ฐ์ํ  ํ์ผ๋ค์ commit์ผ๋ก ์ ์ฅ
  - push๋ก ์๋ก๋ํ๊ธฐ
  ```
  git push origin main
  clear
  ```
  &#8594; git push๋ฅผ ํตํด ๋ก์ปฌ ์ ์ฅ์์ commit์ ๋ณด๋ฅผ ์๊ฒฉ ์ ์ฅ์์ 
  

## ๐ Add Theme on Blog
  - Build Jekyll Project
  - Upload Post
  - Add Theme on Blog<br>
  [jekyll Themes](http://jekyllthemes.org/) ์ฌ์ดํธ๋ฅผ ํตํด์ [Yet Another Them(YAT)](http://jekyllthemes.org/themes/jekyll-theme-yat/) ์ด๋ผ๋ ํ๋ง๋ฅผ ์ด์ฉํ๋ค.
  1. ์ํ๋ ํ๋ง๋ฅผ git cloneํด์ ๋ก์ปฌ์ ๋ฐ์์ค๊ธฐ
  2. _posts๋ฅผ ์ ์ธํ๊ณ  ํ๋ง๋ฅผ ๋ฎ์ด์ฐ๊ธฐ
  3. ๋ณ๊ฒฝ๋ ํ์ผ๋ค์ git์ ๋ฐ์ํ๊ธฐ (git add, git rm)
  
  ๋ ์ฌ์ด ๋ฐฉ๋ฒ: ๋์ ์๊ฒฉ ์ ์ฅ์๋ก ์ํ๋ ํ๋ง์ ์๊ฒฉ ์ ์ฅ์๋ก forkํ ํ,
  ํด๋น ์ ์ฅ์์ ์ด๋ฆ์ <username>.github.io๋ก ๋ณ๊ฒฝ ํ,
  git clone์ ํตํด ๋ฐ์์จ ํ, ์์ ๊ณ์ํ๊ธฐ
  
There are three ways to install:

- As a [gem-based theme](https://jekyllrb.com/docs/themes/#understanding-gem-based-themes).
- As a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/) (GitHub Pages compatible).
- Forking/directly copying all of the theme files into your project.

### Gem-based Theme Method

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-yat"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-yat
```

And then execute:

```bash
$ bundle
```

Or install it yourself as:

```bash
$ gem install jekyll-theme-yat
```

### Remote Theme Method with GitHub Pages

Remote themes are similar to Gem-based themes, but do not require `Gemfile` changes or whitelisting making them ideal for sites hosted with GitHub Pages.

To install:

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "github-pages", group: :jekyll_plugins
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
# theme: owner/name --> Don't forget to remove/comment the gem-based theme option
remote_theme: "jeffreytse/jekyll-theme-yat"
```

And then execute:

```bash
$ bundle
```

### GitHub Pages without limitation

GitHub Pages runs in `safe` mode and only allows [a set of whitelisted plugins/themes](https://pages.github.com/versions/). __In other words, the third-party gems will not work normally__.

To use the third-party gem in GitHub Pages without limitation:

Here is a GitHub Action named [jekyll-deploy-action](https://github.com/jeffreytse/jekyll-deploy-action) for Jekyll site deployment conveniently. ๐
  

## โ๏ธ  Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_data`, `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-theme-yat.gemspec` accordingly.
  
- Support beautiful __Night Mode__.
- Modern responsive web design.
- Full layouts `home`, `post`, `tags`, `archive` and `about`.
- Uses font awesome 5 for icons.
- Beautiful Syntax Highlight using [highlight.js][highlight-js].
- RSS support using [Jekyll Feed][jekyll-feed] gem.
- Optimized for search engines using [Jekyll Seo Tag][jekyll-seo-tag] gem.
- Sitemap support using [Jekyll Sitemap][jekyll-sitemap] gem.
- Complex and flexible table support using [Jekyll Spaceship][jekyll-spaceship] gem.
- MathJAX and LaTeX optional support using [Jekyll Spaceship][jekyll-spaceship] gem.
- Media (Youtube, Spotify, etc.) support using [Jekyll Spaceship][jekyll-spaceship] gem.
- Diagram (PlantUML, Mermaid) support using [Jekyll Spaceship][jekyll-spaceship] gem.
- Google Translation support.
- New post tag support.


<!-- External links -->
[jekyll]: https://jekyllrb.com/
[yat-git-repo]: https://github.com/jeffreytse/jekyll-theme-yat/
[yat-live-demo]: https://jeffreytse.github.io/jekyll-theme-yat/
[jekyll-spaceship]: https://github.com/jeffreytse/jekyll-spaceship
[jekyll-seo-tag]: https://github.com/jekyll/jekyll-seo-tag
[jekyll-sitemap]: https://github.com/jekyll/jekyll-sitemap
[jekyll-feed]: https://github.com/jekyll/jekyll-feed
[highlight-js]: https://github.com/highlightjs/highlight.js
