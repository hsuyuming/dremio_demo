 Step1. Start dremio & mongodb

```bash
docker-compose build
docker-compose up
```

 Step2. Go to http://localhost:9047/ setup dremio

 Step3. Create db and sample data inside mongodb (db:demo collection:tbl)

 Step4. Create mongo connector 
  - name:mongo
  - host:mongodb
  - prot:27017
  - Authentication:No Authentication
  - Authentication database: demo

  Step5. Create snowflake connector
   - name: snowflake
   - jdbc: jdbc:snowflake://<account>.snowflakecomputing.com/?warehouse=<warehouse>
   - username
   - password

