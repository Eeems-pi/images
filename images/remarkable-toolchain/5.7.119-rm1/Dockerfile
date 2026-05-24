FROM eeems/remarkable-toolchain:base

RUN <<EOT
  curl \
    https://storage.googleapis.com/remarkable-codex-toolchain/3.27.0.97/rm1/remarkable-production-image-5.7.119-rm1-public-x86_64-toolchain.sh \
    -o install-toolchain.sh
  echo "dbcedcee5db3e17c62b24132b83cd418e1f0590e1d9e431cb787cf6e798a21cf  install-toolchain.sh" | sha256sum --check
  chmod +x install-toolchain.sh
  ./install-toolchain.sh -y
  rm install-toolchain.sh
EOT
