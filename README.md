# Pcap-_poisoning
Pcap poisoning is a techniques used in manipulating or altering of captured network traffic within a pcap file.

There are two types of Pcap poisoning:
          
	  (i)String Injection where custom strings are injected into a pcap file to hide a file or a 			payload . Attackers use this methods to conceal or hide malware making it difficult 		for standard tools to detect.
		Tools like strings and  grep can be used to identify readable readable text within a 		captures file.
Mostly used in CTF competition to hide flags in a way that requires analysis to retrieve eg injecting a specific string in the HTTP payload of  a PCAP  file that when extracted lead to  a hidden flag.
 
	(ii) Packet Modification , this involve altering the content of existing packets within  the 		PCAP file which include modifying protocol headers(TCP,IP ,,) or packet payloads.
	Tools like scapy or tcpwrite can be used to manipulate packet data including fields like IP 	
	addresses,ports or payloads.
Example of this is changing the destination IP address of a packet to implicate  a different source in a network.
Other type is timestamp manipulation  where you change timestamp of a packet to disrupt the temporary sequence of a network traffic. Tool used is editcap
