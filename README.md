# Awesome-API-Request-History-Audit-Logging

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.



I also have to flag what the search results actually support, because **the open-source side of your list is essentially empty**, and several SaaS entries have no usable pricing.



## The data problems



**LogDNA no longer exists as a standalone product.** IBM acquired LogDNA in 2022 and folded it into **IBM Log Analysis / IBM Cloud Logs**. The search results contain no current LogDNA pricing or product page. **Do not list LogDNA as a current option**—list IBM Cloud Logs if you want the successor.



**The open-source section has almost nothing from your list.** The only genuinely open-source log management project surfaced is **Graylog** (`Graylog2/graylog2-server`) with **7,142 stars**, Java-based, last pushed about a month ago . **Graylog is not in your SaaS list**, but it is the dominant open-source log management platform. **Elastic Logstash** is open source (Java 21, bundled JDK) , but it is a **log pipeline/collector**, not a log management platform with storage and search—it ships logs to Elasticsearch, which is source-available (Elastic License 2.0/SSPL), not OSI open source.



**Postman Request History is a client-side feature, not a log management platform.** It stores sent requests in the sidebar History and migrates from Scratch Pad . It has no server-side retention, search, or audit capabilities comparable to Splunk or Datadog. **Listing it alongside Splunk misleads readers.**



## What the search results actually contain



**Pricing (usable):**

- **Sumo Logic**: Flex pricing—**$0 ingest, unlimited users**, pay per TB scanned. Estimated **$3.14 per TB scanned** for the default profile (500–750 scans/GB) . Credits are consumed by storage and scan volume, not ingest, and there are no overage penalties .

- **Better Stack**: Nano **$25/month annual** ($30 monthly) for 40 GB; Micro **$100/month** (160 GB); Mega **$210/month** (340 GB); Tera **$420/month** (700 GB). Logs & Traces: **$0.10/GB ingestion**, **$0.05/GB/month retention**, **$0.001/GB scanned for query boost** .

- **Coralogix**: **1 unit = $1.50**. Logs high priority: **0.75 units per GB**; medium: **0.32 units/GB**; low: **0.12 units/GB**; blocked: **0.08 units/GB** .

- **Papertrail**: **Starts at $7.00/month**, free plan available .

- **AWS CloudTrail**: First copy of management events to S3 is **free**; additional copies **$2.00 per 100,000 events**; data events **$0.10 per 100,000**; CloudTrail Lake 30-day free trial with 5 GB ingest and 5 GB scan .



**No pricing surfaced for:**

- **Splunk** (results returned only CloudWatch Logs sizing guidance, not Splunk licensing) 

- **Datadog** (results returned only the overage premium structure—**50% premium on on-demand usage above commitment**—not per-GB rates) 

- **Elastic Logstash** (open source, no commercial pricing in results) 



**What is missing:**

- **No star counts** for Graylog beyond the 7,142 figure .

- **No revenue or valuation data** for any vendor.

- **No pricing** for LogDNA (defunct), CloudTrail Logs ingestion (only CloudTrail event delivery) , or Postman Request History .



## What I recommend



**Remove LogDNA** and note it was acquired by IBM. **Remove Postman Request History** from the platform list—it is a client feature, not a log management platform. If you want a Postman-adjacent entry, mention it separately as "API client request history" with no pricing comparison.



**The open-source section should be honest:**



| Project | License | What it actually does | Stars |

|---|---|---|---|

| **Graylog** | Open source (GPL/SSPL per repo) | Log management with storage, search, dashboards | 7,142  |

| **Elastic Logstash** | Open source (Apache 2.0) | Log pipeline/collector—ships to Elasticsearch, not a standalone platform  | Not surfaced |



**There is no open-source equivalent to CloudTrail's audit logging**—CloudTrail is an AWS service, not a deployable product . The closest open-source audit log tooling would be **LogESP** (183 stars, Python SIEM) , but it is not a CloudTrail replacement.



**The SaaS section has usable pricing for Sumo Logic, Better Stack, Coralogix, Papertrail, and CloudTrail.** Splunk and Datadog should be marked **"pricing not surfaced"**—Datadog's overage premium (50%) is documented , but per-GB rates are not.



If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not list LogDNA as current, present Postman Request History as a log management platform, or fabricate Splunk and Datadog per-GB pricing that the results do not support.
