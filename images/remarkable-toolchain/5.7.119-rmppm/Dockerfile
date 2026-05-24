FROM eeems/remarkable-toolchain:base

RUN <<EOT
  curl \
    https://storage.googleapis.com/remarkable-codex-toolchain/3.27.0.97/chiappa/remarkable-production-image-5.7.119-chiappa-public-x86_64-toolchain.sh \
    -o install-toolchain.sh
  echo "f22794bc6bb6729e648a7404a561e870d537818bd62a2f9950522f0cf15b4130  install-toolchain.sh" | sha256sum --check
  chmod +x install-toolchain.sh
  ./install-toolchain.sh -y
  rm install-toolchain.sh
EOT
