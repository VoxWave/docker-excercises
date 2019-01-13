FROM fedora:29
RUN dnf install -y cargo git
RUN git clone https://github.com/VoxWave/dungenon-drawer.git
WORKDIR /dungenon-drawer
RUN cargo build --release
CMD ./target/release/dungenon-drawer