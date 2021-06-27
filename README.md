# Performance testing with Livebook

This repo contains a [Livebook](https://github.com/elixir-nx/livebook) written in Elixir 
that can be used to perform simple API performance/load testing.

- It uses Livebook inputs to set a URL to query + a number of iterations
- It can be easily modified to perform any Elixir funtion, including shelling out with `System.cmd/3` to test any shell function
- It uses [VegaLite](https://github.com/elixir-nx/vega_lite) and [Kino](https://github.com/elixir-nx/kino) to render a graph of response times live as requests are made
- It generates a summary of statistics from the response times and renders it as Markdown
