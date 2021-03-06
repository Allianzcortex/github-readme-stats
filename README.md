# Use

- Update your README

Add a comment to your `README.md` like this:

```md
<!--START_SECTION:my_github-->
<!--END_SECTION:my_github-->
```

- write yml file

[Sample](https://github.com/yihong0618/2021)

```yml
name: GitHub README STATS

on:
  workflow_dispatch:
  schedule:
    - cron: "0 0 * * *"
  push:
    branches:
      - main

env:
  GITHUB_NAME: yihong0618
  GITHUB_EMAIL: zouzou0208@gmail.com
  STARED_NUMBER: 10

jobs:
  build:
    name: Build
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: My GitHub Status
        uses: yihong0618/my_github@v1
        with:
          # if you also want to send TELE
          TELEGRAM_TOKEN: ${{ secrets.TELE_TOKEN }}
          TELEGRAM_CHAT_ID: ${{ secrets.TELE_CHAT_ID }}
          STARED_NUMBER: ${{ env.STARED_NUMBER }}

      - name: Push README
        uses: github-actions-x/commit@v2.6
        with:
          github-token: ${{ secrets.G_T }}
          commit-message: "Refresh README (GITHUB STATUS)"
          files: README.md
          rebase: "true"
          name: ${{ env.GITHUB_NAME }}
          email: ${{ env.GITHUB_EMAIL }}
```



# My example.

## My GitHub Status
<img align="middle" src="https://github-readme-stats-1.yihong0618.vercel.app/api?username=yihong0618&show_icons=true&&&hide_title=true" />

<!--START_SECTION:my_github-->
## The repos I created
| ID |                                    REPO                                    |   START    |   UPDATE   |  LAUGUAGE  | STARS |
|----|----------------------------------------------------------------------------|------------|------------|------------|-------|
|  1 | [running_page](https://github.com/yihong0618/running_page)                 | 2020-09-17 | 2020-12-29 | Python     |   952 |
|  2 | [2020](https://github.com/yihong0618/2020)                                 | 2020-01-10 | 2020-12-29 | C          |    97 |
|  3 | [gaycore](https://github.com/yihong0618/gaycore)                           | 2019-02-18 | 2020-12-10 | Python     |    89 |
|  4 | [gitblog](https://github.com/yihong0618/gitblog)                           | 2019-07-18 | 2020-12-29 | Python     |    77 |
|  5 | [vscode-gcores](https://github.com/yihong0618/vscode-gcores)               | 2020-01-04 | 2020-11-18 | TypeScript |    47 |
|  6 | [shanbay_remember](https://github.com/yihong0618/shanbay_remember)         | 2020-12-02 | 2020-12-28 | JavaScript |    27 |
|  7 | [gcores_calendar](https://github.com/yihong0618/gcores_calendar)           | 2020-08-24 | 2020-12-30 | JavaScript |    19 |
|  8 | [blog](https://github.com/yihong0618/blog)                                 | 2020-06-22 | 2020-12-27 | JavaScript |     9 |
|  9 | [my_github](https://github.com/yihong0618/my_github)                       | 2020-12-24 | 2020-12-30 | Go         |     8 |
| 10 | [Runtastic](https://github.com/yihong0618/Runtastic)                       | 2020-07-24 | 2020-11-16 | Python     |     7 |
| 11 | [Python365](https://github.com/yihong0618/Python365)                       | 2019-09-05 | 2020-10-27 | Python     |     3 |
| 12 | [yihong0618](https://github.com/yihong0618/yihong0618)                     | 2020-07-16 | 2020-12-11 | md         |     1 |
| 13 | [edocteel001](https://github.com/yihong0618/edocteel001)                   | 2019-11-12 | 2020-05-18 | JavaScript |     1 |
| 14 | [2021](https://github.com/yihong0618/2021)                                 | 2020-12-21 | 2020-12-29 | md         |     0 |
| 15 | [hoingyi_bot](https://github.com/yihong0618/hoingyi_bot)                   | 2019-10-16 | 2020-05-25 | Shell      |     0 |
| 16 | [gaycore-server](https://github.com/yihong0618/gaycore-server)             | 2019-02-18 | 2020-11-02 | Go         |     0 |
| 17 | [collections](https://github.com/yihong0618/collections)                   | 2019-03-05 | 2019-03-06 | md         |     0 |
| 18 | [Frontend100](https://github.com/yihong0618/Frontend100)                   | 2019-10-31 | 2019-12-05 | HTML       |     0 |
| 19 | [zouzou0208.github.io](https://github.com/yihong0618/zouzou0208.github.io) | 2018-03-06 | 2018-03-06 | HTML       |     0 |

## The repos I contributed to
| ID |                                   REPO                                    | FIRSTDATE  | LASTEDATE  | PRCOUNT |
|----|---------------------------------------------------------------------------|------------|------------|---------|
|  1 | [GpxTrackPoster](https://github.com/flopp/GpxTrackPoster)                 | 2019-08-06 | 2020-09-26 |       9 |
|  2 | [leetcode-cli](https://github.com/leetcode-tools/leetcode-cli)            | 2019-11-29 | 2020-08-21 |       8 |
|  3 | [vscode-leetcode](https://github.com/LeetCode-OpenSource/vscode-leetcode) | 2019-12-03 | 2020-07-22 |       6 |
|  4 | [nrc-exporter](https://github.com/yasoob/nrc-exporter)                    | 2020-07-05 | 2020-10-07 |       5 |
|  5 | [awesome-cn-cafe](https://github.com/ElaWorkshop/awesome-cn-cafe)         | 2020-08-04 | 2020-08-10 |       3 |
|  6 | [kb](https://github.com/gnebbia/kb)                                       | 2020-09-21 | 2020-09-23 |       3 |
|  7 | [iredis](https://github.com/laixintao/iredis)                             | 2019-12-30 | 2020-09-16 |       2 |
|  8 | [activities](https://github.com/flopp/activities)                         | 2020-07-09 | 2020-07-14 |       2 |
|  9 | [GadioVideo](https://github.com/rabbitism/GadioVideo)                     | 2019-09-25 | 2019-09-25 |       1 |
| 10 | [py-staticmaps](https://github.com/flopp/py-staticmaps)                   | 2020-09-20 | 2020-09-20 |       1 |
| 11 | [LearnJapan](https://github.com/wizicer/LearnJapan)                       | 2020-03-31 | 2020-03-31 |       1 |
| 12 | [highlight](https://github.com/wenyan-lang/highlight)                     | 2020-09-08 | 2020-09-08 |       1 |
| 13 | [build-your-own-vue](https://github.com/jackiewillen/build-your-own-vue)  | 2020-01-16 | 2020-01-16 |       1 |
| 14 | [help-to-be-helped](https://github.com/xiaolai/help-to-be-helped)         | 2020-02-04 | 2020-02-04 |       1 |
| 15 | [awesome-cn-cafe-web](https://github.com/antfu/awesome-cn-cafe-web)       | 2020-08-18 | 2020-08-18 |       1 |
| 16 | [TopList](https://github.com/tophubs/TopList)                             | 2019-08-19 | 2019-08-19 |       1 |

## The repos I stared (random 10)
| ID |                                        REPO                                         | STAREDDATE |     LAUGUAGE     | LATESTUPDATE |
|----|-------------------------------------------------------------------------------------|------------|------------------|--------------|
|  1 | [tile38](https://github.com/tidwall/tile38)                                         | 2020-07-07 | Go               | 2020-12-29   |
|  2 | [pync](https://github.com/SeTeM/pync)                                               | 2019-01-22 | Python           | 2020-12-03   |
|  3 | [im](https://github.com/waylybaye/im)                                               | 2020-08-14 | C++              | 2020-08-23   |
|  4 | [vscode-database](https://github.com/Bajdzis/vscode-database)                       | 2020-01-15 | TypeScript       | 2020-12-17   |
|  5 | [Virgilio](https://github.com/virgili0/Virgilio)                                    | 2019-03-21 | Jupyter Notebook | 2020-12-30   |
|  6 | [Gitter](https://github.com/kokohuang/Gitter)                                       | 2019-06-25 | JavaScript       | 2020-12-28   |
|  7 | [aoc2020](https://github.com/flopp/aoc2020)                                         | 2020-12-02 | Python           | 2020-12-24   |
|  8 | [c9-python-getting-started](https://github.com/microsoft/c9-python-getting-started) | 2019-09-23 | Jupyter Notebook | 2020-12-29   |
|  9 | [youtube](https://github.com/engineer-man/youtube)                                  | 2019-01-24 | Python           | 2020-12-29   |
| 10 | [LearnJapan](https://github.com/wizicer/LearnJapan)                                 | 2019-08-01 | TypeScript       | 2020-12-28   |

<!--END_SECTION:my_github-->
