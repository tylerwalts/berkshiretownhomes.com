# berkshiretownhomes.com

Originally made in 2006.  Restored from archive.org and republished on AWS.

Manual Setup:
* S3 Bucket:
  * Static website configured for root berkshiretownhomes.com, with redirect to www.
* CloudFront Distro:
  * CNAME configured for www.berkshiretownhomes.com
  * Cert created for wildcard `*.berkshiretownhomes.com`
* Route53:
  * `A` root record to S3 redirect to www
  * `CNAME` record for www to CloudFront Distro


