In this reflection, I will be responding to the questions listed in the module 9 page.

**Part 1**

To perform a SBOM analysis on the M5StamPLC, I used the following tools: Syft and Trivy.

![](/images/a.png)<br><center>Screenshot of Syft and Trivy output</center>

Number of components each tool reported:
- Syft: 8 components
- Trivy: 1 component

One key difference between using SPDX SBOM and the CycloneDX SBOM is that SPDX seems to provide a lot more information than CycloneDX. This could be seen in how every component has things like supplier, licenses, and references. 

**Step 2**

When performing a vulnerability analysis on the SBOMs using Grype, I discovered that there are no vulnerabilities in the SBOM.

![](/images/c.png)<br><center>Screenshot of grype output</center>

|CVE|Severity|Component|Version|Comment|
|-|-|-|-|-|
| n/a | n/a | n/a | n/a | n/a |
| n/a | n/a | n/a | n/a | n/a |
| n/a | n/a | n/a | n/a | n/a |
| n/a | n/a | n/a | n/a | n/a |
| n/a | n/a | n/a | n/a | n/a |

The reason why I believe that no CVEs were found were because of a few reasons. One reason could be the reason that Syft discovered no meaningful components and only listed the current directory as a component. This gives very little information to the grype tool. Additionally, there are very little files and dependencies, most of the tools are custom built. For the dependencies that are there, they’re very popular libraries meaning that updates and bug fixes are way more common and prevalent.

