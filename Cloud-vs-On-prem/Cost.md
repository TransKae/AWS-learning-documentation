### What is this document?
In this document, I would like to discuss the pros and cons to on-prem services vs using a cloud service (AWS in this instance) for hosting services to be served to people in an organisation. 

### The difference in payment
This is a point where cloud based may be more appealing to a company, especially one that isn't quite established yet, and doesn't have much money available to them at the time of founding. Cloud based is generally paid in monthly installments whereas buying a server requires an upfront cost for the physical machine itself. Cloud based also means that you do not have to commit to a single machine whereas buying a physical machine involves planning for the future too as it is a commitment that you can't just return or trade-in. Cloud is flexible and allows the administrator to decide what they want at the time based on price and performance required. 

### Analysis of Cloud price
For this first example, we are going to take a very small organisation that needs a server with little computing power (4 vCPUs) and 16gb of RAM. For the cloud option, we are going to use AWS's t3.xlarge EC2 instance. This instance costs $0.1824/hr or £0.14/hr for on-demand instancing at the time of writing. This would work out to £3.36/day or £1227.24/yr (Assuming the average of 365.25 days in a year). Alternatively, this can be brought down to £0.059/hr or £517.194/yr by using AWS's Compute Savings plan in a 3-year contract.
Alternatively, for a more powerful machine with 256gb of RAM and 128 vCPUs such as the AWS c6in.32xlarge, it would cost you £53560.26/yr on demand or £22440.96/yr on a 3-year contract.

### Analysis of On-prem price
Mirroring the examples from the last section, a machine using a current generation CPU with 4 cores and 16gb of DDR5-4800 RAM would cost the following at MSRP:

- CPU: Intel Xeon E-2414 @2.6-4.5GHz - £200 or AMD EPYC 4124P @3.8-5.1GHz - £130 which is much faster and has much better Multithreading capabilities due to hyperthreading.
- RAM: Corsair Vengeance DDR5-4800 2 x 8gb - £85 (much higher right now due to global supply shortages)
- Motherboard: LGA 1700 - £40-100 for low end to midpoint boards. AM5 - £60-100 for equivalents will use midpoint for this example of £70 and £80 respectively.
- Storage: Samsung 980 Pro 256gb - £50 + Seagate Barracuda 2TB - £100
- Other expenses such as PSU, Case, and a UPS if required I would estimate at around £130 without and around £220 with a decent quality UPS.

Going with as cheap as possible, I would use the AMD processor and estimate the price at around £575 without including operating costs.