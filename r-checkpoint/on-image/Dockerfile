FROM rocker/r-ver:devel

ENV CHECKPOINT_DATE 2018-12-01

RUN R -e "install.packages('checkpoint')" && \
    mkdir -p /root/.checkpoint/${CHECKPOINT_DATE} && \
    R -e "library(checkpoint); checkpoint('${CHECKPOINT_DATE}', scanForPackages = FALSE); install.packages(c('shiny', 'rmarkdown'))"

