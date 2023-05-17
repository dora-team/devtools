FROM us-central1-docker.pkg.dev/cloud-workstations-images/predefined/code-oss:latest

# install general-purpose VSCode extensions
RUN wget https://open-vsx.org/api/GitHub/vscode-pull-request-github/0.60.0/file/GitHub.vscode-pull-request-github-0.60.0.vsix && \
unzip GitHub.vscode-pull-request-github-0.60.0.vsix "extension/*" &&\
mv extension /opt/code-oss/extensions/pull-request-github
