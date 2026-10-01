# Package promptx [![Go Reference](https://pkg.go.dev/badge/github.com/davidzchen/promptx.svg)](https://pkg.go.dev/github.com/davidzchen/promptx)

Package promptx is a command line prompt editor with history, kill-ring, and tab
completion. It is a fork of the package `github.com/petermattis/prompt` as the
original is no longer maintained.

The original implementation was inspired by linenoise and derivatives which
eschew usage of terminfo/termcap in favor of treating everything like a VT100
terminal. This is taken a bit further with support for additional input
escape sequences that cover ~75% of the terminals in the terminfo database.
A minimal set of output escape sequences is used for rendering the prompt.
