FROM klakegg/hugo:ext-ubuntu
ARG USERNAME=hugo
ARG USER_UID=1000
ARG USER_GID=$USER_UID

# Create the user mapped to the current user on the host
RUN groupadd --gid $USER_GID $USERNAME \
    && useradd --uid $USER_UID --gid $USER_GID -m $USERNAME

#Set the user
USER $USERNAME