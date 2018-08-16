# Manage dedicated-bandwidth instances {#concept_ezy_mhy_5db .concept}

A dedicated-bandwidth Global Acceleration instance provides a dedicated Internet bandwidth and a public IP for accelerating the Internet access for the added backend service. The bandwidth can only be used by the instance itself.

## Create a dedicated-bandwidth instance {#section_yn4_qhy_5db .section}

After creating a dedicated-bandwidth instance, a public IP is allocated in the region of the instance for accelerating the Internet access. For more information, see [Step 1. Create a Global Acceleration instance](../../../../intl.en-US/Quick Start/Configure a shared-bandwidth Global Acceleration instance.md#section_scl_pxw_5db).

## Bind a backend service {#section_pyj_cly_5db .section}

After creating a dedicated-bandwidth instance, you can bind the backend service that you want to accelerate to the instance directly. The backend service can be bound only to an ECS instance or SLB instance of a VPC network.  For more information, see [Bind a backend service](intl.en-US/User Guide/Dedicated-bandwidth instances/Bind a backend service.md#).

## Unbind a backend service {#section_q4b_vky_5db .section}

You can unbind a backend service from a dedicated-bandwidth instance when acceleration is no longer required. To unbind a backend service, complete these steps:

1.  Log on to the [VPC console](https://vpcnext.console.aliyun.com).
2.  In the left-side navigation pane, click **Global Acceleration**.
3.  Click **Dedicated Bandwidth** and find the target instance.
4.  Click **Unbind** in the **Actions** column.
5.  In the displayed dialog, click **OK**.

## Add an instance name {#section_esj_lky_5db .section}

To add a name for the instance, complete these steps:

1.  Log on to the [VPC console](https://vpcnext.console.aliyun.com).
2.  In the left-side navigation pane, click **Global Acceleration**.
3.  Click **Dedicated Bandwidth** and find the target instance.
4.  Rest the pointer on the instance ID, and then click the displayed pencil icon.
5.  In the displayed dialog box, enter a name and then click **OK**.

    The name can contain 2-128 characters and must start with an English or Chinese character. It can contain numbers, underscores and hyphens.


## Add an instance description {#section_r5q_rky_5db .section}

To add a description for the instance, complete these steps:

1.  Log on to the [VPC console](https://vpcnext.console.aliyun.com).
2.  In the left-side navigation pane, click **Global Acceleration**
3.  Click **Dedicated Bandwidth** and find the target instance.
4.  Rest the pointer on the description area, and then click the displayed pencil icon.
5.  In the displayed dialog box, enter a description and then click **OK**.

    The description can contain 2-256 characters, but cannot start with `http://` or `https://`.


## Modify the bandwidth {#section_itk_lky_5db .section}

You can change the bandwidth of a Global Acceleration instance any time. Changes take effect immediately. To change the bandwidth, complete these steps

1.  Log on to the [VPC console](https://vpcnext.console.aliyun.com).
2.  In the left-side navigation pane, click **Global Acceleration**.
3.  Click **Dedicated Bandwidth** and find the target instance.
4.  Click **Change Bandwidth** in the **Bandwidth** column of the target Global Acceleration instance. Then, select a new bandwidth based on your needs and complete the payment.

## Renew an instance {#section_yqq_dmy_k2b .section}

You must renew a Global Acceleration instance before it expires to avoid a termination of your service. To renew an instance, complete these steps:

1.  Log on to the [VPC console](https://vpcnext.console.aliyun.com).
2.  In the left-side navigation pane, click **Global Acceleration**.
3.  Click **Dedicated Bandwidth** and find the target instance.
4.  Click **Renew** in the **Actions** column.
5.  Select a new time to purchase and complete the payment.

