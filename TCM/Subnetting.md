## 🧠 Subnetting Cheatsheet

| CIDR | Subnet Mask     | Wildcard Mask   | Block Size | Hosts      |
| ---- | --------------- | --------------- | ---------- | ---------- |
| /1   | 128.0.0.0       | 127.255.255.255 | 2147483648 | 2147483646 |
| /2   | 192.0.0.0       | 63.255.255.255  | 1073741824 | 1073741822 |
| /3   | 224.0.0.0       | 31.255.255.255  | 536870912  | 536870910  |
| /4   | 240.0.0.0       | 15.255.255.255  | 268435456  | 268435454  |
| /5   | 248.0.0.0       | 7.255.255.255   | 134217728  | 134217726  |
| /6   | 252.0.0.0       | 3.255.255.255   | 67108864   | 67108862   |
| /7   | 254.0.0.0       | 1.255.255.255   | 33554432   | 33554430   |
| /8   | 255.0.0.0       | 0.255.255.255   | 16777216   | 16777214   |
| /9   | 255.128.0.0     | 0.127.255.255   | 8388608    | 8388606    |
| /10  | 255.192.0.0     | 0.63.255.255    | 4194304    | 4194302    |
| /11  | 255.224.0.0     | 0.31.255.255    | 2097152    | 2097150    |
| /12  | 255.240.0.0     | 0.15.255.255    | 1048576    | 1048574    |
| /13  | 255.248.0.0     | 0.7.255.255     | 524288     | 524286     |
| /14  | 255.252.0.0     | 0.3.255.255     | 262144     | 262142     |
| /15  | 255.254.0.0     | 0.1.255.255     | 131072     | 131070     |
| /16  | 255.255.0.0     | 0.0.255.255     | 65536      | 65534      |
| /17  | 255.255.128.0   | 0.0.127.255     | 32768      | 32766      |
| /18  | 255.255.192.0   | 0.0.63.255      | 16384      | 16382      |
| /19  | 255.255.224.0   | 0.0.31.255      | 8192       | 8190       |
| /20  | 255.255.240.0   | 0.0.15.255      | 4096       | 4094       |
| /21  | 255.255.248.0   | 0.0.7.255       | 2048       | 2046       |
| /22  | 255.255.252.0   | 0.0.3.255       | 1024       | 1022       |
| /23  | 255.255.254.0   | 0.0.1.255       | 512        | 510        |
| /24  | 255.255.255.0   | 0.0.0.255       | 256        | 254        |
| /25  | 255.255.255.128 | 0.0.0.127       | 128        | 126        |
| /26  | 255.255.255.192 | 0.0.0.63        | 64         | 62         |
| /27  | 255.255.255.224 | 0.0.0.31        | 32         | 30         |
| /28  | 255.255.255.240 | 0.0.0.15        | 16         | 14         |
| /29  | 255.255.255.248 | 0.0.0.7         | 8          | 6          |
| /30  | 255.255.255.252 | 0.0.0.3         | 4          | 2          |
| /31  | 255.255.255.254 | 0.0.0.1         | 2          | 2          |
| /32  | 255.255.255.255 | 0.0.0.0         | 1          | 1          |

we created a python tool that will do all the work

```
import ipaddress

def subnet_info(ip_cidr):
    try:
        network = ipaddress.IPv4Network(ip_cidr, strict=False)
    except ValueError as e:
        return f"Error: {e}"

    subnet_mask = network.netmask
    wildcard_mask = ipaddress.IPv4Address(int(network.hostmask))
    total_hosts = network.num_addresses - 2 if network.prefixlen < 31 else network.num_addresses
    first_host = list(network.hosts())[0] if total_hosts >= 1 else "N/A"
    last_host = list(network.hosts())[-1] if total_hosts >= 1 else "N/A"

    result = {
        "IP with CIDR": ip_cidr,
        "Network Address": str(network.network_address),
        "Broadcast Address": str(network.broadcast_address),
        "Subnet Mask": str(subnet_mask),
        "Wildcard Mask": str(wildcard_mask),
        "CIDR": f"/{network.prefixlen}",
        "Total Hosts": total_hosts,
        "Usable Host Range": f"{first_host} - {last_host}" if total_hosts >= 1 else "N/A"
    }

    return result

# Example usage:
if __name__ == "__main__":
    user_input = input("Enter IP/CIDR (e.g. 192.168.1.0/24): ")
    info = subnet_info(user_input)
    
    if isinstance(info, dict):
        print("\n📡 Subnet Info:")
        for key, value in info.items():
            print(f"{key}: {value}")
    else:
        print(info)

```