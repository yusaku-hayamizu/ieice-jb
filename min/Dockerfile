FROM cefore/base
LABEL maintainer="hayamizu <hayamizu@kansai-u.ac.jp>"
WORKDIR /cefore/cefore
RUN ./configure
RUN make
RUN make install
RUN make clean
RUN ldconfig

ENV USER root
COPY ./entrypoint.bash /cefore
ENTRYPOINT /cefore/entrypoint.bash
