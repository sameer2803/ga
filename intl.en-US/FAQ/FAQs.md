# FAQs {#concept_gnr_c4z_5db .concept}

## Q1. When do I need to use Global Acceleration? {#section_n34_f4z_5db .section}

In Alibaba Cloud, a service is deployed in a specific region, while the customers who access the service may not be in this region. For example, customers in Europe may access a service deployed in the China Hangzhou region. In this situation, the region where the service is deployed is a large distance from the region where the customers are. If the quality of the network between the two regions is poor, then high latency, packet loss, jitter, and even inaccessibility may occur, impacting negatively on the customer experience. To solve the problem, Global Acceleration allows customers to bypass the Internet and access the target service through Global Acceleration instances, greatly reducing access latency and improving customer experience.

## Q2. How do I open a Global Acceleration Instance? {#section_o34_f4z_5db .section}

In the pre-release phase, you must apply for and pass the application to purchase and use a Global Acceleration instance. The application site is [http://i.aliyun.com/inviteapply?agent\_id=200](http://i.aliyun.com/inviteapply?agent_id=200).

## Q3. How am I billed for Global Acceleration? {#section_p34_f4z_5db .section}

Global Acceleration supports Subscription billing.

## Q4. Does Global Acceleration charge by bandwidth and charge by traffic? {#section_q34_f4z_5db .section}

A Global Acceleration instance is charged based on the peak bandwidth specified when creating or upgrading the instance. That is, Global Acceleration is charged by bandwidth, not by traffic.

## Q5. If I changed the bandwidth for a Pay-As-You-Go instance, how the fee is charged for that day? {#section_r34_f4z_5db .section}

The fee is based on the highest bandwidth you have set for the day. For example, if the instance bandwidth is set to 10 Mbps, 20 Mbps, and 50 Mbps at different times during the day, the fee that is charged for the day will be based on the cost of 50 Mbps.

## Q6. Which cloud products can serve as the backend servers of a Global Acceleration instance? {#section_s34_f4z_5db .section}

Only ECS instances of the VPC network can serve as the backend servers of a Global Acceleration instance.

## Q7. Which backend server regions does a Global Acceleration instance support? {#section_t34_f4z_5db .section}

When purchasing a Global Acceleration instance, you must specify the region and service area of the Global Acceleration instance. Cloud products to be bound with the Global Acceleration instance and serve as its backend servers can be located only in the regions of the service area and cannot be located in the region of the Global Acceleration instance. For example, if the region of the Global Acceleration instance is China \(Hangzhou\), and the service area of the instance is China Mainland \(including China \(Qingdao\), China \(Beijing\), China \(Shanghai\), and China \(Shenzhen\)\), backend servers to be bound to the Global Acceleration instance can be in China \(Qingdao\), China \(Beijing\), China \(Shanghai\), and China \(Shenzhen\).

## Q8. How many public IPs does a Global Acceleration instance provide? {#section_u34_f4z_5db .section}

A Global Acceleration instance provides one public IP.

## Q9. Where is the public IP of a Global Acceleration instance located? {#section_v34_f4z_5db .section}

The public IP of a Global Acceleration instance is located in the region of the Global Acceleration instance. For example, the public IP of a Global Acceleration instance in China \(Hangzhou\) is also located in Hangzhou. You can configure the public IP according to the actual situation.

## Q10. Is a Global Acceleration instance with no bound backend service charged? {#section_w34_f4z_5db .section}

Yes. After you successfully create a Global Acceleration instance, Alibaba Cloud reserves resources for you and starts charging fees.

## Q11. Why can't I successfully ping the public IP of the Global Acceleration instance after binding the backend service? {#section_x34_f4z_5db .section}

You need to activate the backend service on the ECS instance, that is, configure the backend service IP allocated by the system as a network sub-interface of the ECS instance.

## Q12. When an ECS instance is bound to a Global Acceleration instance, is the access of the ECS instance to the Internet through its public IP, EIP, or NAT Gateway influenced? {#section_y34_f4z_5db .section}

Binding an ECS instance to a Global Acceleration instance does not influence other Internet access methods of the ECS instance. The billing and usage of the Global Acceleration instance is independent from those of the public IP, EIP, or NAT Gateway.

