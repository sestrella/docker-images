FROM sestrella/haskell-base

ENV GHC_VERSION 7.4.2
ENV CABAL_VERSION 1.16

RUN apt-get update && \
    apt-get install -y \
      ghc-$GHC_VERSION \
      cabal-install-$CABAL_VERSION && \
    rm -rf /var/lib/apt/lists/*

ENV PATH /opt/ghc/$GHC_VERSION/bin:$PATH
ENV PATH /opt/cabal/$CABAL_VERSION/bin:$PATH

CMD ["ghci"]
