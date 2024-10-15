tshark -r 0.pcap -Y "ftp" -Tfields -e tcp.payload 2>/dev/null | xxd -ps -r
