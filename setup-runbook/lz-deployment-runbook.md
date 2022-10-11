## What Steps to Take When Deploying The GCP "PBMM" Compliant Landing Zone on Google Cloud
==========================================
gcloud organization list.  (To get 

DIRECTORY_CUSTOMER_ID: Copy this


Policy name: ashumanorgpolicy

Policy id: leave it empty



AUDIT:

additional_user_defined_string = “lbv01”

Bucket name: “lbproductauditlogs”

Sink name: “lb-org-audit-sink-v01”

Bucket viewer: pass your email address

Member user: “your email”

GUARDRAIL:
user_defined_string = “guardrailslbv01”
Billing = your billing

Change group domain to user:your email

org_id_scan_list. = 
{
“Your org id”
}


==========================================

Clone Cloud Source Repository and Copy the Config File to your Current pbmm directory 

= Commit changes to CSR
= PUSH
= The Build Job/Triger for the Common Workload will Automatically get triggered and it’ll deploy the environments (Audit and Security, Workload: Dev, UAT and Prod, Automation, Shared Services, Infrastructure: SharedInfrastructure and Network, Sandbox)