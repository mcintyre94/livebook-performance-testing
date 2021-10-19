[![Run in Livebook](https://livebook.dev/badge/v1/blue.svg)](https://livebook.dev/run?url=https%3A%2F%2Fgithub.com%2Fmcintyre94%2Flivebook-performance-testing%2Fblob%2Fmain%2Fperformance-testing.livemd)

# Performance testing with Livebook

This repo contains a [Livebook](https://github.com/elixir-nx/livebook) written in Elixir 
that can be used to perform simple API performance/load testing.

- It uses Livebook inputs to set a URL to query + a number of iterations
- It can be easily modified to perform any Elixir funtion, including shelling out with `System.cmd/3` to test any shell function
- It uses [VegaLite](https://github.com/elixir-nx/vega_lite) and [Kino](https://github.com/elixir-nx/kino) to render a graph of response times live as requests are made
- It generates a summary of statistics from the response times and renders it as Markdown

## Usage

The easiest way to run this livebook is using livebook.dev: 

[![Run in Livebook](https://livebook.dev/badge/v1/blue.svg)](https://livebook.dev/run?url=https%3A%2F%2Fgithub.com%2Fmcintyre94%2Flivebook-performance-testing%2Fblob%2Fmain%2Fperformance-testing.livemd)

Scroll down to "HTTP request performance testing" which is
where we configure the performance testing.

Update the `URL` and `Iterations` inputs as required.

If required, update the `request_function` definition.
Currently this performs a GET request to the input URL.
This can be any Elixir function, as long as it returns `:ok`

Run the notebook! You can use the keyboard shortcut `ea` to execute all cells.

### Running without livebook.dev

You'll need to install and run Livebook if you don't already have it installed.
Follow the instructions in the repo: https://github.com/elixir-nx/livebook#usage

The notebook can be imported by URL: https://github.com/mcintyre94/livebook-performance-testing/blob/main/performance-testing.livemd


