FROM ghcr.io/lescai-teaching/bigdata-rstudio:latest

ENV NB_USER=rstudio
ENV VIRTUAL_ENV=/opt/venv
ENV PATH=${VIRTUAL_ENV}/bin:${PATH}

RUN /rocker_scripts/install_jupyter.sh

EXPOSE 8888

CMD ["/bin/sh", "-c", "jupyter lab --ip 0.0.0.0 --no-browser"]

USER ${NB_USER}

WORKDIR /home/${NB_USER}
