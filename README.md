# crt.sh-one-liner
Updated crt.sh one liner to get subdomains

  `curl -s https://crt.sh/\?q\=\%.target.com\&output\=json | jq -r '.[].name_value' | sed 's/\*\.//g' | sort -u`
