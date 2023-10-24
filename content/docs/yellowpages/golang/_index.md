---
weight: 10
title: Go Libraries
---

# Go Libraries

## AI & ML

{{< details title="ollama" open=true >}}
Get up and running with Llama 2 and other large language models locally
<br/>{{< sc_github repo="jmorganca/ollama" >}}
{{< /details >}}
<br/>

{{< details title="lingua-go" open=true >}}
The most accurate natural language detection library for Go, suitable for long and short text alike.
It tells you which language some text is written in.
<br/>{{< sc_github repo="pemistahl/lingua-go" >}}
{{< /details >}}
<br/>

## Cache

{{< details title="go-generic-cache" open=true >}}
A key:value store/cache library written in Go generics. LRU, LFU, FIFO, MRU, Clock support.
<br/>{{< sc_github repo="Code-Hex/go-generics-cache">}}
{{< /details >}}
<br/>

{{< details title="bigcache" open=true >}}
Efficient cache for gigabytes of data written in Go.
<br/>{{< sc_github repo="allegro/bigcache">}}
{{< /details >}}
<br/>

{{< details title="clfu" open=true >}}
Implementation of Constant Time LFU (least frequently used) cache in Go with concurrency safety.
<br/>{{< sc_github repo="Narasimha1997/clfu">}}
{{< /details >}}
<br/>

## Compiler & Runtime

{{< details title="gocompiler" open=true >}}
The Go compiler as a package
<br/>{{< sc_github repo="bir3/gocompiler">}}
{{< /details >}}
<br/>

{{< details title="wazero" open=true >}}
wazero: the zero dependency WebAssembly runtime for Go developers
<br/>{{< sc_github repo="tetratelabs/wazero">}}
{{< /details >}}
<br/>

{{< details title="ebitengine/purego" open=true >}}
A library for calling C functions from Go without Cgo.
<br/>{{< sc_github repo="ebitengine/purego">}}
{{< /details >}}
<br/>

## Data structure

{{< details title="GoDS" open=true >}}
GoDS (Go Data Structures) - Sets, Lists, Stacks, Maps, Trees, Queues, and much more
<br/>{{< sc_github repo="emirpasic/gods">}}
{{< /details >}}
<br/>

{{< details title="go-merkletree" open=true >}}
Go Merkle Tree. High performance, Supporting parallel run, OpenZeppelin sorting pairs.
<br/>{{< sc_github repo="txaty/go-merkletree">}}
{{< /details >}}
<br/>

## Database

{{< details title="ramsql" open=true >}}
In-memory SQL engine in Go sql/driver for testing purpose
<br/>{{< sc_github repo="proullon/ramsql">}}
{{< /details >}}
<br/>

{{< details title="rqlite" open=true >}}
The lightweight, distributed relational database built on SQLite
<br/>https://rqlite.io
<br/>{{< sc_github repo="rqlite/rqlite">}}
{{< /details >}}
<br/>

{{< details title="pure go sqlite" open=true >}}
Package sqlite is a CGo-free port of SQLite/SQLite3.
SQLite is an in-process implementation of a self-contained, serverless, zero-configuration, transactional SQL database engine.
<br/>{{< sc_github repo="cznic/sqlite">}}
{{< /details >}}
<br/>

{{< details title="psql-wire" open=true >}}
PostgreSQL server wire protocol. Build your own server and start serving connections.
<br/>{{< sc_github repo="jeroenrinzema/psql-wire">}}
{{< /details >}}
<br/>

{{< details title="slashbase" open=true >}}
Modern database IDE for your dev & data workflows. Supports MySQL, PostgreSQL & MongoDB.
<br/>{{< sc_github repo="slashbaseide/slashbase">}}
{{< /details >}}
<br/>

{{< details title="pocketbase" open=true >}}
Open Source realtime backend in 1 file
<br/>{{< sc_github repo="pocketbase/pocketbase">}}
{{< /details >}}
<br/>

{{< details title="rosedb" open=true >}}
Lightweight, fast and reliable key/value storage engine based on Bitcask.
<br/>{{< sc_github repo="rosedblabs/rosedb">}}
{{< /details >}}
<br/>

{{< details title="milvus" open=true >}}
A cloud-native vector database, storage for next generation AI applications.
Milvus is an open-source vector database built to power embedding similarity search and AI applications. 
<br/>{{< sc_github repo="milvus-io/milvus">}}
{{< /details >}}
<br/>

{{< details title="column" open=true >}}
High-performance, columnar, in-memory store with bitmap indexing in Go
<br/>{{< sc_github repo="kelindar/column">}}
{{< /details >}}
<br/>

{{< details title="LinDB" open=true >}}
Distributed time-series db
https://lindb.io
{{< /details >}}
<br/>

{{< details title="m3db" open=true >}}
M3 monorepo - Distributed TSDB, Aggregator and Query Engine, Prometheus Sidecar, Graphite Compatible, Metrics Platform
<br/>{{< sc_github repo="m3db/m3">}}
{{< /details >}}
<br/>

## Datetime

{{< details title="carbon" open=true >}}
A simple, semantic and developer-friendly golang package for datetime.
<br/>{{< sc_github repo="golang-module/carbon">}}
{{< /details >}}
<br/>

## Event & Message driven

{{< details title="watermil" open=true >}}
Go library for building event-driven applications.
https://watermill.io
{{< /details >}}
<br/>

{{< details title="RxGo" open=true >}}
Reactive Extensions for the Go language.
<br/>{{< sc_github repo="reactivex/rxgo">}}
{{< /details >}}
<br/>

## Interpreter & Evaluation

{{< details title="expr" open=true >}}
Expression language and expression evaluation for Go
<br/>{{< sc_github repo="antonmedv/expr">}}
{{< /details >}}
<br/>

## Game

{{< details title="cardrank" open=true >}}
Go types, funcs, and utilities for working with cards, decks, and evaluating poker hands (Holdem, Omaha, Stud, more)
<br/>{{< sc_github repo="cardrank/cardrank">}}
{{< /details >}}
<br/>

## GUI

{{< details title="go-app" open=true >}}
A package to build progressive web apps with Go programming language and WebAssembly.
<br/>{{< sc_github repo="maxence-charriere/go-app">}}
{{< /details >}}
<br/>

{{< details title="gio ui" open=true >}}
Gio is a library for writing cross-platform immediate mode GUI-s in Go. Gio supports all the major platforms: Linux, macOS, Windows, Android, iOS, FreeBSD, OpenBSD and WebAssembly.
https://gioui.org
{{< /details >}}
<br/>

## Kafka

{{< details title="kafka-go" open=true >}}
Kafka library in Go
<br/>{{< sc_github repo="segmentio/kafka-go">}}
- sarama, which is by far the most popular but is quite difficult to work with. It is poorly documented, the API exposes low level concepts of the Kafka protocol, and it doesn't support recent Go features like contexts. It also passes all values as pointers which causes large numbers of dynamic memory allocations, more frequent garbage collections, and higher memory usage.
- confluent-kafka-go is a cgo based wrapper around librdkafka, which means it introduces a dependency to a C library on all Go code that uses the package. It has much better documentation than sarama but still lacks support for Go contexts.
- goka is a more recent Kafka client for Go which focuses on a specific usage pattern. It provides abstractions for using Kafka as a message passing bus between services rather than an ordered log of events, but this is not the typical use case of Kafka for us at Segment. The package also depends on sarama for all interactions with Kafka.
{{< /details >}}
<br/>

{{< details title="sarama" open=true >}}
Sarama is a Go library for Apache Kafka.
<br/>{{< sc_github repo="IBM/sarama">}}
{{< /details >}}
<br/>

{{< details title="confluent-kafka-go" open=true >}}
Confluent's Apache Kafka Golang client
<br/>{{< sc_github repo="confluentinc/confluent-kafka-go">}}
{{< /details >}}
<br/>

{{< details title="goka" open=true >}}
Goka is a compact yet powerful distributed stream processing library for Apache Kafka written in Go.
<br/>{{< sc_github repo="lovoo/goka">}}
{{< /details >}}
<br/>

## Log

{{< details title="tint" open=true >}}
🌈 slog.Handler that writes tinted (colorized) logs
<br/>{{< sc_github repo="lmittmann/tint">}}
{{< /details >}}
<br/>

{{< details title="log" open=true >}}
A minimal, colorful Go logging library 🪵
<br/>{{< sc_github repo="charmbracelet/log">}}
{{< /details >}}
<br/>

{{< details title="tail" open=true >}}
Go package for reading from continously updated files (tail -f)
<br/>{{< sc_github repo="hpcloud/tail">}}
{{< /details >}}
<br/>

{{< details title="zincsearch" open=true >}}
ZincSearch . A lightweight alternative to elasticsearch that requires minimal resources, written in Go.
<br/>{{< sc_github repo="zincsearch/zincsearch">}}
{{< /details >}}
<br/>

## macOS

{{< details title="gon" open=true >}}
Sign, notarize, and package macOS CLI tools and applications written in any language. Available as both a CLI and a Go library.
<br/>{{< sc_github repo="mitchellh/gon">}}
{{< /details >}}

## Media

{{< details title="go2rtc" open=true >}}
Ultimate camera streaming application with support RTSP, RTMP, HTTP-FLV, WebRTC, MSE, HLS, MP4, MJPEG, HomeKit, FFmpeg, etc.
<br/>{{< sc_github repo="AlexxIT/go2rtc">}}
{{< /details >}}
<br/>

{{< details title="Livekit (WebRTC)" open=true >}}
End-to-end stack for WebRTC. SFU media server and SDKs.
<br/>{{< sc_github repo="livekit/livekit">}}
{{< /details >}}
<br/>

## Monitoring

{{< details title="goalive" open=true >}}
A simple tool to monitor health endpoints of your services
<br/>{{< sc_github repo="Stef2k16/goalive">}}
{{< /details >}}

## Network

{{< details title="quic-go" open=true >}}
A QUIC implementation in pure go
<br/>{{< sc_github repo="quic-go/quic-go">}}
{{< /details >}}
<br/>

{{< details title="ws" open=true >}}
Tiny WebSocket library for Go.
<br/>{{< sc_github repo="gobwas/ws">}}
{{< /details >}}
<br/>

{{< details title="torrent" open=true >}}
Full-featured BitTorrent client package and utilities
<br/>{{< sc_github repo="anacrolix/torrent">}}
{{< /details >}}
<br/>

{{< details title="loxilb" open=true >}}
eBPF based cloud-native load-balancer. Powering K8s|Edge|5G|IoT|XaaS Apps.
<br/>{{< sc_github repo="loxilb-io/loxilb">}}
{{< /details >}}
<br/>

{{< details title="natiu-mqtt" open=true >}}
A dead-simple, extensible MQTT implementation well suited for embedded systems.
<br/>{{< sc_github repo="soypat/natiu-mqtt">}}
{{< /details >}}
<br/>

{{< details title="comqtt" open=true >}}
A lightweight, high-performance go mqtt server(v3.0|v3.1.1|v5.0) supporting distributed cluster
<br/>{{< sc_github repo="wind-c/comqtt">}}
{{< /details >}}
<br/>

{{< details title="easytcp" open=true >}}
✨ 🚀 EasyTCP is a light-weight TCP framework written in Go (Golang), built with message router. EasyTCP helps you build a TCP server easily fast and less painful.
<br/>{{< sc_github repo="DarthPestilane/easytcp">}}
{{< /details >}}
<br/>

## OpenStreetMap

{{< details title="openmaptiles" open=true >}}
OpenMapTiles Vector Tile Schema Implementation
<br/>{{< sc_github repo="openmaptiles/openmaptiles">}}
{{< /details >}}
<br/>

{{< details title="tegola-omt" open=true >}}
OpenMapTiles import procedure and configuration for the Tegola tileserver.
<br/>{{< sc_github repo="tile-fund/tegola-omt">}}
{{< /details >}}
<br/>

## Security

{{< details title="life4/enc" open=true >}}
🔑🔒 A modern and friendly CLI alternative to GnuPG: generate and download keys, encrypt, decrypt, and sign text and files, and more.
<br/>{{< sc_github repo="life4/enc">}}
{{< /details >}}
<br/>

{{< details title="go-nanoid" open=true >}}
Nano ID for Go
<br/>{{< sc_github repo="jaevor/go-nanoid">}}
{{< /details >}}
<br/>

## Terminal

{{< details title="console" open=true >}}
Closed-loop application library for Cobra commands (powerful, ready-to-run and easy to use)
<br/>{{< sc_github repo="reeflective/console">}}
{{< /details >}}
<br/>

{{< details title="pterm" open=true >}}
PTerm is a modern Go module to easily beautify console output. Featuring charts, progressbars, tables, trees, text input, select menus and much more 🚀 It's completely configurable and 100% cross-platform compatible.
<br/>{{< sc_github repo="pterm/pterm">}}
{{< /details >}}
<br/>

{{< details title="command line interactive libraries" open=true >}}
- readline : {{< sc_github repo="chzyer/readline">}}
- go-prompt : {{< sc_github repo="c-bata/go-prompt">}}
- prompt-ui : {{< sc_github repo="manifoldco/promptui">}}
- gosh : https://medium.com/@vladimirvivien/gosh-a-pluggable-command-shell-in-go-cf25102c8439
- sshportal : {{< sc_github repo="moul/sshportal">}}
- winpty : {{< sc_github repo="iamacarpet/go-winpty">}}
- sshd example: https://gist.github.com/jpillora/b480fde82bff51a06238
{{< /details >}}
<br/>

{{< details title="go-pretty" open=true >}}
Table-writer and more in golang!
<br/>{{< sc_github repo="jedib0t/go-pretty">}}
{{< /details >}}
<br/>

{{< details title="artty" open=true >}}
Art for your TTY.
<br/>{{< sc_github repo="mjwhitta/artty">}}
{{< /details >}}
<br/>

{{< details title="banner" open=true >}}
Colorful Banners
- figlet : displays the banners
- lolcat : colorizes the banners
{{< /details >}}
<br/>

## Utilities

{{< details title="go-git" open=true >}}
A highly extensible Git implementation in pure Go.
<br/>{{< sc_github repo="go-git/go-git">}}
{{< /details >}}
<br/>

{{< details title="duf" open=true >}}
Disk Usage/Free Utility - a better 'df' alternative
<br/>{{< sc_github repo="muesli/duf">}}
{{< /details >}}
<br/>

{{< details title="zellij" open=true >}}
A terminal workspace with batteries included
https://zellij.dev
{{< /details >}}
<br/>

## Visualization

{{< details title="D2" open=true >}}
D2 is a modern diagram scripting language that turns text to diagrams
<br/>{{< sc_github repo="terrastruct/d2">}}
{{< /details >}}
<br/>

{{< details title="go-echarts" open=true >}}
🎨 The adorable charts library for Golang
<br/>{{< sc_github repo="go-echarts/go-echarts">}}
{{< /details >}}
<br/>

{{< details title="uPlot" open=true >}}
📈 A small, fast chart for time series, lines, areas, ohlc & bars
<br/>{{< sc_github repo="leeoniya/uPlot">}}
{{< /details >}}
<br/>
