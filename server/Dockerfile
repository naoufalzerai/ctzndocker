FROM node:14-slim
ARG DOMAIN
RUN npm install -g ctzn
RUN echo $DOMAIN
RUN env
CMD ["ctzn", "start", "--domain", "$DOMAIN"]
