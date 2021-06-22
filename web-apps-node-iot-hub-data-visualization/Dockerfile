FROM node:12

WORKDIR /usr/src/app

COPY package*.json ./

RUN set IoTHubConnectionString=Endpoint=sb://abbaashub.servicebus.windows.net/;SharedAccessKeyName=webapp;SharedAccessKey=HRIA6MsCg+JmuLKDuuvVQ3MEcuVY23bAojC5pKqO5lA=;EntityPath=iotevents
RUN set EventHubConsumerGroup=$Default
RUN npm install 

COPY . .

EXPOSE 3000


CMD ["npm","start"]