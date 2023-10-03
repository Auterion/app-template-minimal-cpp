FROM auterion/app-base:v2

WORKDIR /buildroot
COPY /src/CMakeLists.txt /buildroot/
COPY /src/{{cookiecutter.app_name}}.cpp /buildroot/

RUN mkdir -p /buildroot/build && \
    cd /buildroot/build && \
    cmake .. && \
    make
WORKDIR /
RUN mkdir app && cp /buildroot/build/{{cookiecutter.app_name}} app

ENTRYPOINT [ "/app/{{cookiecutter.app_name}}"]

