# mevn-opentelemetry-example

### Installing packages
Clone the repo locally & follow these steps

**Server**:
</br>
</br>
Get into `/server` folder & install packages

```
cd server
npm i

```

**Client:**
</br>
</br>
Get into `/client` folder & install packages

```
cd client
npm i

```

### Running the application
Get into the `server` folder.

```
cd server

```

Before running the server, create a MongoDB connection and get the mongodb_uri. 
Set the `MONGO_URI` & `PORT` in `.env` (check `.env.exmaple` for reference)
Finally, run the following command to start both `server` and `client`

```
npm run dev

```

### Running SigNoz
Get into `./signoz` folder.

```
cd signoz/deploy
./install.sh

```

Run the following commands to set these env variables

```
export OTEL_EXPORTER_OTLP_ENDPOINT="http://localhost:4317"
export OTEL_RESOURCE_ATTRIBUTES=service.name=mevn-signoz

```
