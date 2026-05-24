FROM eeems/remarkable-toolchain:base

RUN <<EOT
  curl \
    https://storage.googleapis.com/remarkable-codex-toolchain/3.27.0.97/rm2/remarkable-production-image-5.7.119-rm2-public-x86_64-toolchain.sh \
    -o install-toolchain.sh
  echo "7ac74daf817ec9d0c52bcaec9f23b1d3ec5cf7e5a41f58e1d739fb54fbf947d4  install-toolchain.sh" | sha256sum --check
  chmod +x install-toolchain.sh
  ./install-toolchain.sh -y
  rm install-toolchain.sh
EOT
