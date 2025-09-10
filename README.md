# OCaml Nostr Client

This is a simple Nostr client written in OCaml. It connects to a Nostr relay, subscribes to events, and prints `kind: 1` (short text notes) events to the console.

This project demonstrates how to use the [piaf](https://github.com/anmonteiro/piaf) library to create a WebSocket client in OCaml.

## Prerequisites

- [OCaml](https://ocaml.org/docs/install)
- [Dune](https://dune.build/)
- [OPAM](https://opam.ocaml.org/)

## Setup

1.  Install the required OCaml libraries:

    ```bash
    opam install piaf yojson eio
    ```

## Build

To build the project, run the following command:

```bash
dune build
```

## Run

To run the client, execute the following command:

```bash
dune exec piaf-nostr-client
```

The client will connect to the relay specified in `bin/main.ml` and start printing `kind: 1` events.
