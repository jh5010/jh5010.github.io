<div align="center">
  <br>

  <h1>나의 GitBlog </h1>

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


<h3 align="center">🌌 Night Mode</h3>

<p align="center">

  <img src="https://user-images.githubusercontent.com/9413601/94983351-760f6e00-0574-11eb-9494-5303ad6228dc.gif" alt="demo-screenshot" width="780px"/>

</p>

## ✨ Git 시작하기
  
  - Git 로컬 저장소 생성
  ```
  user $ git init
  ```
  &#8594; 현재 작업중인 디렉토리를 git 저장소로 지정하기
  
  - Git에 변경사항 반영하기
  ```
  user $ git status
  ```
  &#8594; 현재 Git 상태 확인
  
  ```
  user $ git add example.py
  ```
  &#8594;example.py를 생성/수정하고, 이를 Commit에 반영하고 싶은 경우
  
  ```
  user $ git commit -m "add example.py"
  ```
  &#8594; 변경사항이 반영된 new commit 생성
  
  ```
  user $ git log
  ```
  &#8594; commit 기록 확인하기 (Author, Commitor, Date, ...)
  
  - Git Branch 생성
  ```
  user $ git branch <branch_name>
  ```
  &#8594; git branch를 생성
  
  ```
  user $ git checkout <branch_name>
  ```
  &#8594; 현재 작업중인 branch를 전환
  
  ```
  user $ git merge <branch_name>
  ```
  &#8594; 현재 작업중인 branch를 원하는 branch에 병합
  
  ```
  user $ git branch -d <branch_name>
  ```
  &#8594; branch를 삭제

## 🛠️  Github Repo를 Webpage로 만들기
  - Github Page 시작하기
  1. Repository 생성<br>
    Github에서 <username>.github.io 이름의 Repo 생성<br>
  2. Local-Remote Repository 연동<br>
    생성한 Repo에서 Remote Repository의 주소 복사<br>
    ```
    git clone <repo_name> <path>
    ```<br>
    &#8594; git clone으로 클론하기<br>
  3.예시 문서 작성<br>
    예시 파일(index.html) 작성<br>
  4. git commit 남기기<br>
    ```
    git status
    git add
    ```<br>
    &#8594; git status로 현재 상태 확인 후 git add로 변경파일 추가<br>
    ```
    git commit -m "msg"
    ```<br>
    &#8594; 커밋 남기기<br>
  5. git push로 원격 저장소에 반영하기<br>
    ```
    git branch -M main
    ```<br>
    &#8594; 현재 branch의 이름을 main으로 변경<br>
    ```
    git status
    git add index.html
    ```<br>
    &#8594; git status로 현재 상태 확인 후 git add로 변경파일 추가<br>
    ```
    git push origin main
    ```<br>
    &#8594; git push를 통해 원격저장소에 반영<br>
    &#8594; Password에 PAT(Personal Access Token)을 입력하여 git push하기<br>
  6. Github Page 설정 확인<br>
    &#8594; Repository Settings > Pages > 중간에 있는 주소(username.github.io) 접속<br>
    &#8594; 이전에 입력한 HTML 문서가 잘 뜨면 성공<br>
  
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

Here is a GitHub Action named [jekyll-deploy-action](https://github.com/jeffreytse/jekyll-deploy-action) for Jekyll site deployment conveniently. 👍
  
## ✏️ Build Jekyll Project
  &#8594 Local Repository에서 Jeykll 시작 후, 원격 저장소에 이를 반영하기
  - Requisite
  ```
  jekyll -v
  ```
  &#8594 Jekyll이 설치되어있는지 확인
  - Start Jekyll
  ```
  jekyll new . --force
  ```
   &#8594 현재 디렉토리(.).에 Jekyll 설치
  ```
  bundle exec jekyll serve
  ```
  &#8594 (bundle exec) jekyll serve 실행 후, localhost:4000 접속

## 📚 Add Theme on Blog
  - Build Jekyll Project
  - Upload Post
  - Add Theme on Blog<br>
  [jekyll Themes](http://jekyllthemes.org/) 사이트를 통해서 [Yet Another Them(YAT)](http://jekyllthemes.org/themes/jekyll-theme-yat/) 이라는 테마를 이용했다.
  1. 원하는 테마를 git clone해서 로컬에 받아오기
  2. _posts를 제외하고 테마를 덮어쓰기
  3. 변경된 파일들을 git에 반영하기 (git add, git rm)
  
  더 쉬운 방법: 나의 원격 저장소로 원하는 테마의 원격 저장소로 fork한 후,
  해당 저장소의 이름을 <username>.github.io로 변경 후,
  git clone을 통해 받아온 후, 작업 계속하기
  

## ✏️  Development

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
