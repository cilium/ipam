This repo is a fork of `k8s.io/kubernetes/pkg/registry/core/service` package.

This is useful if repositories want to use this library without importing
`k8s.io/kubernetes` repository.

All of the functions remain untouched except `func (r *Range) Snapshot()` for
which that function was re-written to avoid importing `k8s.io/kubernetes/pkg/apis/core`.
