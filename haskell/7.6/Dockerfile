FROM sestrella/haskell-base

ENV GHC_VERSION 7.6.3
ENV CABAL_VERSION 1.18

RUN apt-get update && \
    apt-get install -y \
      ghc-$GHC_VERSION \
      cabal-install-$CABAL_VERSION && \
    rm -rf /var/lib/apt/lists/*

ENV PATH /opt/ghc/$GHC_VERSION/bin:$PATH
ENV PATH /opt/cabal/$CABAL_VERSION/bin:$PATH
