# MPIL GitHub Webpage (with Jekyll)


## Development Environment (Windows 11)
Refer to [this blog](https://present4n6.tistory.com/7), [this blog](https://balabala.tistory.com/75), and [this blog](https://myung-ho.tistory.com/89)


### Install Ruby
Install Ruby first WITH DEVKIT (for Windows).
For now, I have installed Ruby+Devkit 3.2.2-1 (x64).

Check Ruby version in cmd:
```bash
# check Ruby version
D:\github_local_repository\mpil-gist.github.io>ruby -v
# ruby 3.2.2 (2023-03-30 revision e51014f9c0) [x64-mingw-ucrt]

# check RubyGems version
D:\github_local_repository\mpil-gist.github.io>gem -v
# 3.4.10
```


### Install Jekyll
Simply run the following
```bash
gem install bundler jekyll
```

Check jekyll and bundler version in cmd:
```bash
# check jekyll version
D:\github_local_repository\mpil-gist.github.io>jekyll -v
# jekyll 4.3.2

# check bundler version
D:\github_local_repository\mpil-gist.github.io>bundler -v
# Bundler version 2.4.19
```


## Running a Server
You can run a local server as follows:
```bash
bundle exec jekyll serve
```

If it is your first time running a server, execute the below before running a server.
```bash
bundle install
```
