**ESP32-S3FN8**

Manufacturer: Xtensa

Part number or chip family: ESP32-S3FN8

Known vulnerabilities or operational risk:

* CVE-2025-53540
* CVE-2025-53094
* CVE-2025-53007
* CVE-2025-27840
* CVE-2024-45798
* CVE-2023-6249
* CVE-2023-35818
* CVE-2021-34173
* CVE-2021-28139
* CVE-2021-28136
* CVE-2021-28135
* CVE-2020-13595
* CVE-2020-13594
* CVE-2019-17391
* CVE-2019-15894

**ST7789V2**

Manufacturer: Sitronix

Part number or chip family: ST7789V2

Known vulnerabilities or operational risk: None found

If a vulnerability is found, it could send commands to neighboring chips to exfiltrate data. Also could maliciously affect what is being displayed

**LM75B**

Manufacturer: NXP Semiconductors

Part number or chip family: LM75B

Known vulnerabilities or operational risk: None found

If a vulnerability is found, it could open the device to corrupt temperature readings from this chip. This could affect features such as watchdog services.

**Summarize how hardware dependencies can influence firmware/software risk (supply-chain discussion)**

When people conduct penetration or vulnerability assessments, they focus on the device or object at hand and don’t usually consider what the device is made up of. If a device is found to be safe from vulnerabilities, say in its software, backdoors or vulnerabilities could still exist in the chips themselves. This exponentially expands the attack vector since an attacker could look at a HBOM and target those chips; in essence find the weakest link. These hardware dependencies should be heavily inspected as much as software dependencies. 
