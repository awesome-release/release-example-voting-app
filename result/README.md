| **Sub-heading**       | **Instruction / Value**                                                                                                                                                                                                        |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Base Image**        | node:18-alpine                                                                                                                                                                                                                 |
| **Work Directory**    | /app                                                                                                                                                                                                                           |
| **Port**              | 80                                                                                                                                                                                                                             |
| **Launch Command**    | node server.js                                                                                                                                                                                                                 |
| **Build Instruction** | npm config set registry [https://registry.npmjs.org](https://registry.npmjs.org) 
                          npm install -g nodemon
 
                          npm install \
                      <br> && npm ls \
                      <br> && npm cache clean --force \
                      <br> && mv /app/node_modules /node_modules 

