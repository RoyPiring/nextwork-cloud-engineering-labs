<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** Roy Piring Jr  
**Email:** rpiringhawaii@gmail.com

---

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

This project provisions a static website hosted on Amazon S3. The system uses S3 object storage to serve HTML and static assets directly over HTTP without application servers or compute resources.

### Tools and concepts

The implementation focuses on S3 static website hosting capabilities. S3 is used as an object store with public read access scoped to website assets, functioning as a simple content origin rather than a general-purpose file server.

### Time, challenges, and wins

This implementation is intentionally minimal. The scope is limited to validating static hosting behavior, permissions, and access patterns rather than optimizing for scale, security hardening, or production traffic.

---

## How I Set Up an S3 Bucket

### What I did in this step

The S3 bucket provides the storage boundary for website content and defines the namespace for all hosted objects.

### How long it took to create the bucket

Bucket creation establishes the container required for static website hosting.

### Region selection

The bucket is created in the us-west-1 region to control data residency and endpoint location. Region selection affects latency, pricing, and the generated website endpoint.

### Understanding bucket name uniqueness

S3 bucket names are globally unique because they are part of the public DNS namespace. This constraint prevents naming collisions across all AWS accounts and regions.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

The website consists of an index.html file and supporting image assets stored as S3 objects. These files represent the full application surface for a static site.

### Files I uploaded

Both files are required for correct site rendering.

### How the files work together

S3 serves the HTML document and referenced assets directly to clients without server-side processing.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

Static website hosting configures S3 to serve objects over an HTTP endpoint. The bucket is designated with an index document and optional error document to define request handling behavior.

### Understanding website hosting

Access control determines whether objects are publicly readable.

### How I enabled website hosting

Public access must be explicitly allowed through bucket configuration while balancing security risks.

### Access Control Lists (ACLs)

An ACL defines object-level permissions that control who can read or write individual objects. ACLs are legacy mechanisms and interact with bucket-level access settings.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Enabling static website hosting generates a region-specific S3 website endpoint. This endpoint provides unauthenticated HTTP access to objects configured for public read.

### What I saw when I tested the endpoint

Initial access to the endpoint returned an error due to insufficient public access permissions. The bucket and object access configuration prevented anonymous reads.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

The access issue was resolved by correcting permissions that blocked public reads.

### How I resolved the 403 error

Once access controls aligned with static website requirements, the site rendered successfully through the S3 endpoint.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

Bucket policies are JSON documents that define access rules for S3 buckets and objects. They apply at the bucket level and support centralized, explicit permission management.

### Understanding bucket policies

Policies can enforce security controls such as restricting actions, limiting principals, or requiring specific conditions.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

In this configuration, the policy restricts object deletion, including deletion attempts by the bucket owner.

---

---
