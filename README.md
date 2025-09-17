Wireshark SSH Traffic Analysis
Project Overview

This project demonstrates how to analyze SSH traffic using Wireshark.
I used a sample .pcapng file containing SSHv2 connections and applied filters to isolate the traffic on port 22.

Steps

Downloaded a sample SSH.pcapng capture file.

Opened the file in Wireshark.

Applied the filter:

tcp.port == 22


to view only SSH traffic.

Used Statistics → Conversations → TCP tab to identify the top talkers.

Findings

The most active SSH conversation was between:

192.168.2.2 (client)

200.1.1.2 (server, SSH port 22)

A total of 230 packets were exchanged (~28 KB of data).

Most of the packets originated from the client (192.168.2.2).

Tools Used

Wireshark (traffic analysis)

Key Learning

This project shows how Wireshark can be used to identify SSH communication patterns, the volume of packets exchanged, and the top participants in a network session.


