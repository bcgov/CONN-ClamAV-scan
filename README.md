[![Lifecycle:Experimental](https://img.shields.io/badge/Lifecycle-Experimental-339999)](Redirect-URL)

# AWS ClamAV Lambda Layer 

based on https://github.com/sutt0n/serverless-clamav-lambda-layer

# How to build locally

```
git clone https://github.com/bcgov/CONN-ClamAV-scan
./build.sh
```

After successfult `build.sh` execution,  archive `clamav_lambda_layer.zip` would be generated in the ./layer folder.
Archive contains fresh virus definiotion and thus it is too big to be included in the terraform lambda deployment script; it has to to be uploaded to S3 and referenced by the terraform.
