# GitHub Polls

User polls for GitHub powered by [Up](github.com/apex/up).

[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20A)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20A/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20B)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20B/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20C)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2T00TMSDTZWJ1RP6TQF200/Option%20C/vote)

## About

These polls work by pasting individual markdown SVG images into your issue, each wrapped with a link that tracks a vote. A single vote per IP is allowed for a given poll, which are stored in DynamoDB.

What do they look like? The poll above is live, click one out and give it a try! Please don't abuse it or I'll have to take it down :).

## Installation

Via `go get`:

```
$ go get github.com/tj/gh-polls/cmd/polls
```

## Usage

Create a new poll for who is the best ferret.

```
$ polls new Tobi Loki Jane
```

[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Tobi)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Tobi/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Loki)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Loki/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Jane)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z07AGE7KBMK8T2RFJCBWY/Jane/vote)

Create a new poll with larger options.

```
$ polls new "Cats are better" "Ferrets are better"
```

[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z0HTHT9P5TXGREGP1T29F/Cats%20are%20better)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z0HTHT9P5TXGREGP1T29F/Cats%20are%20better/vote)
[![](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z0HTHT9P5TXGREGP1T29F/Ferrets%20are%20better)](https://m131jyck4m.execute-api.us-west-2.amazonaws.com/prod/poll/01BM2Z0HTHT9P5TXGREGP1T29F/Ferrets%20are%20better/vote)

---

[![GoDoc](https://godoc.org/github.com/tj/gh-polls?status.svg)](https://godoc.org/github.com/tj/gh-polls)
![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-experimental-orange.svg)

<a href="https://apex.sh"><img src="http://tjholowaychuk.com:6000/svg/sponsor"></a>
