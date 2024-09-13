# DEPLOYMENT AWS PROCESS PROJECT

## Endpoint FE Web and BE API

- Frontend: <http://udacity-deployment.s3-website-us-east-1.amazonaws.com/>
- Backend: <http://longpt-udacity.us-east-1.elasticbeanstalk.com/api/v0>

## Dependencies

- Both application using NodeJS version 16.16.0

- FrontEnd - WEB
   angular version 8.x.x
   iconic-native version 5.x.x

- Backend - API
   express version 4.x.x
   pg version 8.x.x
   aws-sdk version 2.429.0

## AWS Setup

### AWS RDS

- Database Host: postgres.cfdxl9gkha8y.us-east-1.rds.amazonaws.com
- Database Port: 5432
- Database Name: postgres

### AWS S3 Bucket

- S3 Endpoint: <http://udacity-deployment.s3-website-us-east-1.amazonaws.com>
- Resource Name: arn:aws:s3:::udacity-deployment

### AWS Elastic Beanstalk

- Application name: longpt-udacity
- Environment name: longpt-udacity-env
- Running platform: Node.js 16 running on 64bit Amazon Linux 2/5.9.6

## Environment Variables

Add those variables into .env file or cloud environment:

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_SESSION_TOKEN
- AWS_BUCKET
- AWS_REGION
- AWS_PROFILE
- AWS_DEFAULT_REGION
- POSTGRES_USERNAME
- POSTGRES_PASSWORD
- POSTGRES_HOST
- POSTGRES_DB
- JWT_SECRET

## Scripts

From the root folder, run the following script

### Frontend

```json
   - Install: npm run frontend:install
   - Run application: npm run frontend:start
   - Build application: npm run frontend:build
   - Deploy npm run frontend:deploy
```

### Backend

```json
   - Install: npm run api:install
   - Run application: npm run api:start
   - Build application: npm run api:build
   - Deploy npm run api:deploy
```

### Both

```json
   - To build both application: npm run api:build
   - To deploy both application: npm run deploy
```
