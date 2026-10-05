FROM mcr.microsoft.com/playwright:v1.39.0-jammy

RUN apt-get update && \
    apt-get install -y curl && \
    curl -fsSL https://deb.nodesource.com/setup_20.x | bash - && \
    apt-get install -y nodejs && \
    rm -rf /var/lib/apt/lists/*

RUN npm install -g netlify-cli@20.1.1 serve

RUN apt-get update && \
    apt-get install -y jq && \
    rm -rf /var/lib/apt/lists/*