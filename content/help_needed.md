---
tags: [ecosystem]
---

# Help Needed

Are you looking to help the OCaml ecosystem, but not sure where to start?
This page should give you some ideas of where the community
thinks work is needed.

It's worth keeping in mind that making the ecosystem just a little more usable,
especially at critical points, can have massive implications downstream.

## Documentation

- [odoc](https://github.com/ocaml/odoc/tree/master/src/odoc) (needs help, *high priority*):
the new standard documentation tool for OCaml.
Unfortunately, it still needs some love -- check out the Issues.
This is a great place to contribute since a little effort on the documentation
front can go a long way.
- doc.ocaml.org (non-existent):
We need to have a central site for documentation of all packages.
Odoc already does a good job on package documentation generation.
We would like the CI infrastructure to build docs for each package as it tests it.

## Web and Networking

- [gRPC](https://grpc.io/): no support.
There is an [issue](https://github.com/grpc/grpc/issues/14251) in the official
project.
There is also a discussion on the [OCaml discourse](https://discuss.ocaml.org/t/grpc-implementation-in-ocaml/1624).

- Elasticsearch (needs help): the defacto standard search solution.
[ocaml-elasticsearch](https://github.com/skydeck/ocaml-elasticsearch) is
abandoned.

- GraphQL client (needs help):
Having [ppx_graphql](https://github.com/andreas/ppx_graphql)
support the full [GraphQL spec](http://facebook.github.io/graphql/June2018/)
opens up the possibility to interact with many APIs that expose a GraphQL
endpoint including Github.

## GUI

- [LablGTK3](https://github.com/garrigue/lablgtk) (needs help) - not yet feature
complete as GTK2 state, see `lablgtk3` branch.

## Machine Learning

- [OWL](https://github.com/owlbarn/owl) (needs help):
OCaml's equivalent to Numpy and Pytorch.
Currently, the project doesn't support GPUs, which hurts its adoption by
machine learning professionals.

## Cloud Technology

- [Google Cloud Platform](https://cloud.google.com/apis/): no bindings.
- [NATS/NATS Streaming](https://nats.io/): no bindings.
Part of the [Cloud Native Foundation](https://www.cncf.io/) and gaining increased adoption.

## Discord-IRC Bridge bot

- Our IRC to Discord bot doesn't work well, and the bridge is currently broken.
We'd much prefer to have a Discord library in OCaml, and possibly a bot creation library.
[This](https://github.com/jerith/chaocaml) may be a good starting point.
