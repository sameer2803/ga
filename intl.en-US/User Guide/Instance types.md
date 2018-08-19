# Instance types {#concept_f3w_q3x_5db .concept}

Global Acceleration provides two kinds of instance types: dedicated-bandwidth instances and shared-bandwidth instances.

## Dedicated-bandwidth instances {#section_ppv_v3x_5db .section}

A dedicated-bandwidth Global Acceleration instance provides a dedicated Internet bandwidth and a public IP for accelerating the Internet access of the backend service. A dedicated-bandwidth Global Acceleration instance provides a dedicated Internet bandwidth and a public IP for accelerating the Internet access for the added backend service. The bandwidth of a dedicated-bandwidth instance is exclusively used by the Global Acceleration instance itself. The bandwidth is used only by the instance itself.

After creating a dedicated-bandwidth instance, you can bind the backend service to it directly.

## Shared-bandwidth instances {#section_vyp_1jx_5db .section}

A shared-bandwidth Global Acceleration instance provides a shared Internet bandwidth, but does not provide a public IP.

You can add one or more Elastic IP Addresses \(EIPs\) to a shared-bandwidth instance.  After they are added, the EIPs can be used to accelerate the Internet access for the backend services. Additionally, the EIPs share the bandwidth of the shared-bandwidth instance to reduce the Internet cost.

The regions of the backend services that the EIPs are bound to must be the same.

A shared-bandwidth instance allows you to separately manage IP and bandwidth, and has the following benefits:

-   Cost effectiveness

    The EIPs added to a shared-bandwidth instance share the instance, reducing the Internet cost.

-   Flexible management

    When you want to change the public IP of your service, instead of purchasing a new Global Acceleration instance, you can unbind the EIP from the backend service and then bind a new EIP to the backend service.

-   Cross-region binding

    The EIP added to a shared-bandwidth instance can bind to a backend service that is in a different region from the EIP.


## Dedicated-bandwidth instances vs. Shared-bandwidth instances {#section_pyl_pkx_5db .section}

|Items|Dedicated-bandwidth instances|Shared-bandwidth instances|
|:----|:----------------------------|:-------------------------|
|Bind backend services in different regions| Yes.

 You can bind the backend services in different regions to a dedicated-bandwidth instance directly.

 | Yes.

 After adding an EIP to a shared-bandwidth instance, the EIP can bind to a backend service in a different region.

 |
|Share the bandwidth of the instance|No.|Yes|
|Public IP|A public IP is allocated to a dedicated-bandwidth instance for accelerating the Internet access.|No public IP is allocated to a shared-bandwidth instance. You must add one or more EIPs to the instance for accelerating the Internet access.|
|Supported backend services|ECS and SLB instances of the VPC network.|ECS secondary ENI and SLB instances of the VPC network.|

