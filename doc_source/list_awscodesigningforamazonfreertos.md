# Actions, Resources, and Condition Keys for AWS Code Signing for Amazon FreeRTOS<a name="list_awscodesigningforamazonfreertos"></a>

AWS Code Signing for Amazon FreeRTOS \(service prefix: `signer`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/signer/latest/developerguide/Welcome.html)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/signer/latest/api/)\.

**Topics**
+ [Actions Defined by AWS Code Signing for Amazon FreeRTOS](#awscodesigningforamazonfreertos-actions-as-permissions)
+ [Resources Defined by Signer](#awscodesigningforamazonfreertos-resources-for-iam-policies)
+ [Condition Keys for AWS Code Signing for Amazon FreeRTOS](#awscodesigningforamazonfreertos-policy-keys)

## Actions Defined by AWS Code Signing for Amazon FreeRTOS<a name="awscodesigningforamazonfreertos-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ CancelSigningProfile ](https://docs.aws.amazon.com/signer/latest/api/API_CancelSigningProfile.html)  | Cancels a signing profile\. | Write |  |  |  | 
|   [ DescribeSigningJob ](https://docs.aws.amazon.com/signer/latest/api/API_DescribeSigningJob.html)  | Describe a signing job\. | Read |  |  |  | 
|   [ GetSigningPlatform ](https://docs.aws.amazon.com/signer/latest/api/API_GetSigningPlatform.html)  | Retrieves a signing platform\. | Read |  |  |  | 
|   [ GetSigningProfile ](https://docs.aws.amazon.com/signer/latest/api/API_GetSigningProfile.html)  | Retreives a signing profile\. | Read |  |  |  | 
|   [ ListSigningJobs ](https://docs.aws.amazon.com/signer/latest/api/API_ListSigningJobs.html)  | List signing jobs\. | List |  |  |  | 
|   [ ListSigningPlatforms ](https://docs.aws.amazon.com/signer/latest/api/API_ListSigningPlatforms.html)  | List all signing platforms\. | List |  |  |  | 
|   [ ListSigningProfiles ](https://docs.aws.amazon.com/signer/latest/api/API_ListSigningProfiles.html)  | List all signing profile associated with the account\. | List |  |  |  | 
|   [ PutSigningProfile ](https://docs.aws.amazon.com/signer/latest/api/API_PutSigningProfile.html)  | Creates a new signing profile if not exists\. | Write |  |  |  | 
|   [ StartSigningJob ](https://docs.aws.amazon.com/signer/latest/api/API_StartSigningJob.html)  | Starts a code signing request\. | Write |   [ signing\-profile\* ](#awscodesigningforamazonfreertos-signing-profile)   |  |  | 

## Resources Defined by Signer<a name="awscodesigningforamazonfreertos-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awscodesigningforamazonfreertos-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ signing\-profile ](https://docs.aws.amazon.com/signer/latest/developerguide/Welcome.htmlpermissions.html)  |  arn:$\{Partition\}:signer:$\{Region\}::/signing\-profiles/$\{profileName\}  |  | 

## Condition Keys for AWS Code Signing for Amazon FreeRTOS<a name="awscodesigningforamazonfreertos-policy-keys"></a>

Signer has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.