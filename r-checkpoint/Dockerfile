FROM rocker/r-ver:3.6.1

ENV CHECKPOINT_DATE 2018-12-01

RUN R -e "install.packages('checkpoint')" && \
    mkdir -p /root/.checkpoint/${CHECKPOINT_DATE} && \
    echo "library(checkpoint); checkpoint('${CHECKPOINT_DATE}', scanForPackages = FALSE);" >~/.Rprofile && \
    R -e "install.packages('colorspace')"

