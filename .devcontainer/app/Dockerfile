FROM mcr.microsoft.com/devcontainers/dotnet:1-8.0-bookworm

ARG USERNAME=vscode
RUN SNIPPET="export PROMPT_COMMAND='history -a' && export HISTFILE=/commandhistory/.bash_history" \
    && mkdir /commandhistory \
    && touch /commandhistory/.bash_history \
    && chown -R $USERNAME /commandhistory \
    && echo "$SNIPPET" >> "/home/$USERNAME/.bashrc"

WORKDIR /workspaces/BlazorAzureADB2CApp1
