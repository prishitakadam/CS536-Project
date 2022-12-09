# Reproducing "An argument for increasing TCP’s initial congestion window"

## Introduction

## Experiments
<details>
<summary><b>Impact of Congestion Window size on Latency</b></summary>
Add here
</details>

<details>
<summary><b>Impact of Congestion Window size on Latency in Lossless and Lossy networks</b></summary>
Add here
</details>

<details>
<summary><b>Impact on subnets of varying BW, RTT and BDP</b></summary>
Add here
</details>

<details>
<summary><b>Impact on subnets of varying the number of segments</b></summary>
Add here
</details>

## Limitations
The primary reason for an increase in latency is due to packet losses caused by overflowing bottleneck buffers. TCP flows are prolonged due to these losses as they add extra RTTs that are required to recover lost packets. This may also occasionally result in retransmission timeouts. The retransmission rate of TCP represents an upper bound for the percentage of packets lost as a result of congestion. We conducted an experiment to measure the impact of init_cwnd=10 on the retransmission rate. We calculated the average retransmission rate for initial congestion windows 3, 10, and 16 for payloads of different sizes. We found that as the value of the initial congestion window increases the average retransmission rate also increases. This is because the effective burst size transmitted is larger for a higher initial congestion window which in case results in an increased retransmission rate.
