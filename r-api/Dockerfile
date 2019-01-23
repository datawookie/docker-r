FROM r-base

RUN apt-get update && \
    apt-get install -y -qq \
        libcurl4-openssl-dev \
        libssl-dev \
        libgit2-dev

RUN R -e 'install.packages(c("devtools", "jsonlite", "dplyr", "tidyr", "readxl", "writexl", "stringr", "here", "rlang", "forcats", "plumber"))'

