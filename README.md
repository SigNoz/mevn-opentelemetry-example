# mevn-opentelemetry-example

### Installing packages
Clone the repo locally & follow these steps

**Server**:
```
cd server
npm i

```

**Client:**
```
cd client
npm i

```
### Running the application

```
cd server
npm run dev

```
Before runnning the application, create a MongoDB connection and set the `.env` using `.env.exmaple`

### Running SigNoz

```
cd signoz/deploy
./install.sh

```

Run the following commands to set these env variables

```
export OTEL_EXPORTER_OTLP_ENDPOINT="http://localhost:4317"
export OTEL_RESOURCE_ATTRIBUTES=service.name=mevn-signoz

```
