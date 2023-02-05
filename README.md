- Apply your changes to documentation in this folder and commit and push
- Run docker-compose up -d --build
- Run docker-exec -it docs bash
- Within docker clone the current repo and build new docs
  ```
  git clone https://github.com/STEELISI/CLASSNET-DOCS.git
  cd CLASSNET-DOCS
  mkdocs build
  mkdocs gh-deploy (requires auth)
  ```
  
