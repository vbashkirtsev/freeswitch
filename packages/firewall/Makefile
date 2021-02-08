all:
	iptables-restore < /etc/iptables

	# H.323 Gatekeeper RAS port
	iptables -I INPUT  6 -p udp --dport 1719 -j ACCEPT

	# H.323 Call Signaling
	iptables -I INPUT  7 -p tcp --dport 1720 -j ACCEPT

	# MSRP
	iptables -I INPUT  8 -m multiport -p tcp --dports 2855:2856 -j ACCEPT

	# STUN service
	iptables -I INPUT  9 -m multiport -p udp --dports 3478:3479 -j ACCEPT

	# MLP protocol server
	iptables -I INPUT 10 -p tcp --dport 5002 -j ACCEPT

	# Neighborhood service
	iptables -I INPUT 11 -p udp --dport 5003 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 12 -m multiport -p udp --dports 5060:5061 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 13 -m multiport -p tcp --dports 5060:5061 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 14 -m multiport -p udp --dports 5070:5071 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 15 -m multiport -p tcp --dports 5070:5071 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 16 -m multiport -p udp --dports 5080:5081 -j ACCEPT

	# SIP UAS
	iptables -I INPUT 17 -m multiport -p tcp --dports 5080:5081 -j ACCEPT

	# ESL
	iptables -I INPUT 18 -p tcp --dport 8021 -j ACCEPT

	# RTP/ RTCP multimedia streaming
	iptables -I INPUT 19 -m multiport -p udp --dports 16384:32768 -j ACCEPT

	# Websocket
	iptables -I INPUT 20 -p tcp --dport 5066 -j ACCEPT

	# Websocket
	iptables -I INPUT 21 -p tcp --dport 7443 -j ACCEPT

	# Websocket
	iptables -I INPUT 22 -m multiport -p tcp --dports 8081:8082 -j ACCEPT

	# HTTP for CertBot
	iptables -I INPUT 23 -p tcp --dport 80 -j ACCEPT

	# HTTPS for CertBot
	iptables -I INPUT 24 -p tcp --dport 443 -j ACCEPT

	iptables-save -f /etc/iptables
