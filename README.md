# donovan-said.github.io

This website was built using [Jekyll](https://jekyllrb.com/) and the 
[portfolYOU](https://github.com/YoussefRaafatNasry/portfolYOU/tree/master) theme.

# Local Testing

## With Docker

Using method defined by [Bret Fisher](https://github.com/BretFisher/jekyll-serve).

```shell
docker build -t donovan-said-github-io:latest .
docker-compose up

```

## Without Docker

```shell
bundle install
bundle exec jekyll serve
```
