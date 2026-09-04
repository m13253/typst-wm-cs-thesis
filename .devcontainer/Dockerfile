FROM ghcr.io/typst/typst as typst

FROM mcr.microsoft.com/devcontainers/base
COPY --from=typst /bin/typst /bin
