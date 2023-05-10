FROM us-central1-docker.pkg.dev/cloud-workstations-images/predefined/code-oss:latest

# install general-purpose VSCode extensions
# RUN /opt/code-oss/bin/codeoss-cloudworkstations --install-extension GitHub.vscode-pull-request-github
RUN wget https://open-vsx.org/api/GitHub/vscode-pull-request-github/0.60.0/file/GitHub.vscode-pull-request-github-0.60.0.vsix
RUN /opt/code-oss/bin/codeoss-cloudworkstations --install-extension GitHub.vscode-pull-request-github-0.60.0.vsix
