This is the entry point for theme architect!

- Depending on the theme you choose, entry point differs.
- here entry point is set by naming the file as `index.md`
- Simple pages are set by just creating markdown files as [First Simple Page](first-simple-page) and [Second Simple Page](second-simple-page)
- Posts are defined by setting is frontmatter `layout:default` in architect theme. Posts can also be made by soimply creating a markdown file.
- As in theme minimal or minima, the posts are not automatically showing in the entering page We have to link it uisng `<a></a>` tags like below:
  - [First Simple Page](first-simple-page)
  - [Second Simple Page](second-simple-page)
  - [First Default Page](first-default-page)

## **Pre-requisites:**

- Ruby installed (For windows - [https://rubyinstaller.org/downloads/](https://rubyinstaller.org/downloads/)), the one with devkit
- jekyll and bundler installed - `gem install jekyll bundler`

## **Process:**

- **Create a `_config.yml`**
  - For properties, visit [https://json.schemastore.org/jekyll.json](https://json.schemastore.org/jekyll.json). In that go to the key called properties and under it every key is a possible property that can be added to the config file.
  - For default properties specific to any particular theme or website template, visit that template and read its documentation or code base to identiy what variables are used in its code.
  - Finding variables :
  - <img src='https://github.com/user-attachments/assets/04612ac5-0aba-45f2-8b2e-fdea9d482f74' width='400'/>
  - <img src='https://github.com/user-attachments/assets/045f61eb-3b55-407a-9ace-a021514d1913' width='400'/>
  - We will be using architect theme from [https://github.com/pages-themes/architect](https://github.com/pages-themes/architect). I'll just go ahead and copy info from its `_config.yml`
- **Create a file called `Gemfile`**
  - Its like package.json but for ruby. It contains gems (packages for installation)
  - In it add necessary gems for jekyll, and those related to the respective theme/template. ([example]())
  - Bundle the gemfile by running `bundle install` or just `bundle`
- **Create a file called `.gitignore`** specific to jekyll, automatically by running `npx gitignore jekyll`
- **Adding files**:
  - Add a readme file that acts a starting point
  - Add markdown posts in a folder named `_posts`. Posts must be name in format `yyyy-mm-dd-title.md`. ([example]())
  - Add additonal [frontmatter](https://jekyllrb.com/docs/front-matter/) to any post or page that you make. ([example]())
  - Add custom markdown pages [optional]. (example)
  - Add custom html pages [optional]. (example)
  - Add custom html components [optional]. (example)

## **Running:**

- Running webpage locally: run `bundle exec jekyll serve`
- Running webpage with github: push to repo and setup github pages via settings
