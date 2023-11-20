This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).


## Create a .env file
Please do not use NEXT_PUBLIC_

```bash
AWS_S3_REGION=eu-west-2
AWS_S3_ACCESS_KEY_ID=
AWS_S3_SECRET_ACCESS_KEY=
AWS_S3_BUCKET_NAME=
```

## Run the project

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## S3 Tutorial Policy

You can find example policies here [https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html](AWS S3 DOCS) with your browser to see the result.

```bash
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::gearxplorer-prod/*"
        }
    ]
}
```


