# GitHub-Trending-Crawler

Crawling [GitHub Trending Pages](https://github.com/trending/) if you click star or run at actions page.

## Introduction

The program is highly recommend to be deployed on Github Actions, which can crawl information about popular repositories of languages you are interested in on GitHub every day. Then it will create a markdown file to record those information.

This crawler is designed to help me keep track of the latest trends in technology and discover some new and interesting repositories. In fact, reading the newest markdown file has become a part of my daily routines. More importantly, it increases contributions of GitHub :P

The idea was inspired by [LJ147](https://github.com/LJ147/GithubTrending).

## Requirements

+   Github PAT saved as secret(at repo settings page) named `GH_TOKEN`.

## Configuration

First,[Generate](https://github.com/rdp-studio/GitHub-Trending-Crawler/generate) form [This Repo](https://github.com/rdp-studio/GitHub-Trending-Crawler),then active GitHub Pages and Github Actions for your repo,then edit line 137 in file crawler.py for your own infomation with this temeplete`f.write('<script type="text/javascript">window.location.href="https://[GITHUB USER NAME].github.io/[GITHUB REPO NAME]/' + today_date + '.html";</script>\n')`,then run the action in the actions page,init complete.It will automaticly run when you click on star.

## Change Logs

### V2.5 (2021-02-11)

+ Refactor code with object-oriented methods
+ Split single python file into several files
+ Improve exception handling
+ Add logging feature
+ Use `docopt` to enhance command-line usage
+ Update requirements
+ Use Github Actions for one click run
