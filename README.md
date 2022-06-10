# go-solid
Experimenting

Idea: Enterprise-ready SOLID server written in golang

Requirements
- must use an object store like S3 or equivalent (should not use a local file system)
- must implement the specification completely
- must not have features that go beyond the specification (like a spar-QL engine)

## Why do this?
- I believe in the solid project and want it to become bolstered by a healthy market for pods and apps. For this to happen, the barrier to entry for private pod providers needs to come down. We can reduce that berrier by providing an efficient, enterprise-ready server. Pod providers can build differentiation on top of an enterprise-grade foundation.

## There are already open-source SOLID servers, why do we need another one?
- At the time of writing, there are really two open source implementations: NSS (node solid server) and SCS (solid community server). Both of these projects are great, but their target consumer is not enterprise, and therefor they are not likely to be chosen by private-sector teams. TODO: elaborate on my reasons for saying this.
