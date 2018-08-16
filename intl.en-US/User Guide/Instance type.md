# Instance type {#concept_f3w_q3x_5db .concept}

Global Acceleration provides dedicated-bandwidth instances and shared-bandwidth instances.

## Dedicated-bandwidth instance {#section_ppv_v3x_5db .section}

A dedicated-bandwidth Global Acceleration instance provides a dedicated Internet bandwidth and a public IP for accelerating the Internet access of the backend service. The bandwidth of a dedicated-bandwidth instance is exclusively used by the Global Acceleration instance itself.

## Shared-bandwidth instance {#section_vyp_1jx_5db .section}

A shared-bandwidth Global Acceleration instance only contains an Internet bandwidth without any public IP.

You can add one or more Elastic IP Addresses \(EIPs\) to a shared-bandwidth instance. After adding, the EIPs can be used to accelerate the Internet access of the backend services. Additionally, the EIPs share the bandwidth of the shared-bandwidth instance and the Internet cost is reduced.

The regions of the backend services that the EIPs are bound must be the same.

The shared-bandwidth instance provides you with the capability to separately manage IP and bandwidth and has the following benefits:

-   Cost effectiveness

    The EIPs added to a shared-bandwidth instance share the bandwidth of the instance and save the bandwidth cost.

-   Flexible management

    When you want to change the IP address of your service, you only need to unbind the EIP from the instance \(ECS ENI or SLB\), and bind the instance with another EIP added to the shared-bandwidth instance. You do not need to buy a new Global Acceleration instance.

-   Cross-region binding

    After adding to a shared-bandwidth instance, the EIP can bind a backend service in any region of the service area.


## Dedicated-bandwidth instances versus shared-bandwidth instances {#section_pyl_pkx_5db .section}

|Items|Dedicated-bandwidth instance|Shared-bandwidth instance|
|:----|:---------------------------|:------------------------|
|Bind a backend service in different regions| Yes.

 You can directly bind a dedicated-bandwidth instance to a backend service in another region.

 | Yes

 The EIP added to a shared-bandwidth instance can bind the backend service in any region of the service area.

 |
|Share the bandwidth of the instance|No.|Yes.|
|Public IP|The dedicated-bandwidth instance provides a public IP for accelerating the Internet access.|The shared-bandwidth instance does provide a public IP. Elastic IP Address \(EIP\) is used for accelerating the Internet access.|
|Supported services|ECS instances and SLB instances of the VPC network.|ECS secondary ENI and SLB instances of the VPC network.|

