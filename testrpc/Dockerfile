FROM node:10

# expose to the 8545 port
ENV PORT 8545

# installing the dependencies 
RUN npm install -g --unsafe-perm ganache-cli && \
    npm install -g truffle && \
    npm set progress=false

# start the testrpc
CMD ["ganache-cli", "-m 'help maple me bake pudding cream honey rich smooth crumble sweet treat'"]