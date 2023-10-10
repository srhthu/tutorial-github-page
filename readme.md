# Tutorial of Building Github Pages
Github Pages can host static site. You can build your personal website, project documentations and blogs.

To publish a repository, go to `Settings/Pages` to config. For example, the repository `https://github.com/srhthu/tutorial-github-page` will be published at `https://srhthu.github.io/tutorial-github-page`. Each github account can publish unlimited repositories but only one user page.

## Philosophy
### Basic
Github page will render the default html file `index.html` in the repository. It can accessed other files, e.g., `main.css` or `index.js` through the relative position.

> It may take several minutes to update changes. The building progress can be viewed under `Actions`

### Render with Front-end Framework
The page can be built by frameworks:
- Jekyll (recommended by github) [Github doc](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)
- vue
- react
- angular
- hexo: blog framework. [web](https://hexo.io/index.html)

The repository should be initialized by the corresponding tools.
```Bash
# To create a new Jekyll site
jekyll new --skip-bundle .

# To create a vue + webpack project
vue init webpack github-page-vue-demo
```

**Change Build Source**
The default build source is the master branch. It can be changed to the `docs` folder if exists.

It is useful if you want to build a document website for your project. The repository can include project codes under the `<proj_name>` folder and website files under `docs`.

### Others
- badges. [license](https://gist.github.com/lukas-h/2a5d00690736b4c3a7ba); [a web intro](https://www.freecodecamp.org/news/how-to-use-badges-to-stop-feeling-like-a-noob-d4e6600d37d2/)