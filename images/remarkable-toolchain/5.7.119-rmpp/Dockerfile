FROM eeems/remarkable-toolchain:base

RUN <<EOT
  curl \
    https://storage.googleapis.com/remarkable-codex-toolchain/3.27.0.97/ferrari/remarkable-production-image-5.7.119-ferrari-public-x86_64-toolchain.sh \
    -o install-toolchain.sh
  echo "324d77d84dda5ba8fac484107b3c9981daaa28fe5ebed6589172f0cb1bcdd020  install-toolchain.sh" | sha256sum --check
  chmod +x install-toolchain.sh
  ./install-toolchain.sh -y
  rm install-toolchain.sh
EOT
