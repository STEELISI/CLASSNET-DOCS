- Apply your changes to documentation in this folder and commit and push
- First time, run `docker-compose up -d --build`
- Run `docker-exec -it docs bash`
- Within docker clone the current repo and build new docs
  ```
  git clone https://github.com/STEELISI/CLASSNET-DOCS.git
  cd CLASSNET-DOCS
  mkdocs build
  mkdocs gh-deploy (requires auth)
  ```
- You do not have to rebuild Docker container and clone repository, each time you change docs. Just
run `docker-exec it docs bash` and then do `cd CLASSNET-DOCS` followed by `git pull`. Then continue with `build` and `gh-deploy`.
