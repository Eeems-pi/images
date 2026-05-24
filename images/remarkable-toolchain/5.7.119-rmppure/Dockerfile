FROM eeems/remarkable-toolchain:base

RUN <<EOT
  curl \
    https://storage.googleapis.com/remarkable-codex-toolchain/3.27.0.97/tatsu/remarkable-production-image-5.7.119-tatsu-public-x86_64-toolchain.sh \
    -o install-toolchain.sh
  echo "165d9f090a8bece2e8df695adb606cd7146c1b76699be3d530c0f23105264dd5  install-toolchain.sh" | sha256sum --check
  chmod +x install-toolchain.sh
  ./install-toolchain.sh -y
  rm install-toolchain.sh
EOT
