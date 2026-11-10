### Nobuo Otoi — cybersecurity research, Tokyo

Independent cybersecurity researcher in Tokyo, publishing as [ba-cybersecurity.com](https://ba-cybersecurity.com/research/).

**Main line — web application firewalls.** How OWASP CRS and managed WAFs produce false positives, and how to predict the effect of a configuration change before it is deployed. Prospective validation is in preparation. Meanwhile [WAF Rule Watch](https://ba-cybersecurity.com/radar/waf/) tracks public WAF rule updates daily and is listed in [Awesome-WAF](https://github.com/0xInfection/Awesome-WAF).

#### Recent results

Errors found in two IETF documents already approved for publication (SUIT, CRI) and in one individual draft (ASRA), each shown with a counterexample and answered by an author on the IETF list; flaws reported to widely used software and fixed; published cryptanalysis values improved or corrected.

| | |
|---|---|
| [SUIT (IETF)](https://ba-cybersecurity.com/research/suit-version-comparison/) | A firmware version condition for a final release also accepted its pre-releases. Hand-checkable counterexample; an author confirmed the error, and revision -17 (2 Nov 2026) changed the encoding. [Code](https://github.com/otoinobuo/suit-verify) |
| [CRI (IETF CoRE)](https://ba-cybersecurity.com/research/cri-reference-resolution/) | One reference could resolve to two different addresses: 3 mismatches with RFC 3986, with counterexamples and fixes. An author replied that the necessary corrections will be made. [Code](https://github.com/otoinobuo/cri-verify) |
| [ASPA and ASRA (IETF SIDROPS)](https://ba-cybersecurity.com/research/aspa-asra-verification/) | ASPA route-leak detection proved correct in Lean 4 for paths of any length; the proposed ASRA extension can mark a correct route Invalid. Counterexample and proved fix; the lead author replied that the algorithms will be re-checked. [Code](https://github.com/otoinobuo/aspa-verify) |
| [FreeRADIUS](https://ba-cybersecurity.com/research/freeradius-teap/) | TEAP could accept a client without verifying any MAC. Reproduced and reported; fixed in source (v3.2.x), credited in the commit. |
| [Langfuse](https://ba-cybersecurity.com/research/langfuse-organization-invite/) | Any member, whatever their role, could invite users into the organization by naming a project of another organization. Reported; fixed and listed in the Hall of Fame on Langfuse's responsible-disclosure page. |
| [ARADI (NSA cipher)](https://ba-cybersecurity.com/research/aradi-6r-optimum/) | In CLAASP's model, the best six-round differential trail has weight 82, not the 84 that Table 4 of *CLAASPing ARADI* prints as optimal; lower bound from 945 DRAT-checked subproblems. Not an attack. [Code](https://github.com/otoinobuo/aradi-6r-optimum) |
| [Ascon](https://ba-cybersecurity.com/research/ascon-active-sboxes/) | Characteristics with fewer active S-boxes than the best published ones we found: 42 over 4 rounds (was 43), 68 over 5 (was 72). Not an attack. [Code](https://github.com/otoinobuo/ascon-trails) |
| [ECDSA weak-key rule (CA/B Forum draft ballot)](https://ba-cybersecurity.com/research/ecdsa-scalar-rule/) | The proposed rule rejects private scalars below 256 but accepts n − k and k⁻¹, recovered by the same search at the same cost. Keys derived from the eight eMudhra incident keys; Lean 4 proof. The drafter agreed they are as easy to attack but declined the change, citing no real-world cases. [Code](https://github.com/otoinobuo/ecdsa-scalar-verify) |

All results and their status: [ba-cybersecurity.com/research](https://ba-cybersecurity.com/research/)

#### Papers and talks

| | |
|---|---|
| [What the Inbox Remembers: Receiver-Side Longitudinal Measurement of Email Authentication and Inbound TLS, 2005–2026](https://ssrn.com/abstract=7552629) | Preprint, SSRN, October 2026 |
| [Hidden to Whom? Invisible Text in Ordinary HTML Email and the Rules Against It](https://doi.org/10.21203/rs.3.rs-11230329/v1) | Preprint, Research Square, November 2026 |
| [How Often Do Spam Filters' Hidden-Text Rules Flag Current Benign HTML Email?](https://ba-cybersecurity.com/research/hidden-text-benign-email/) | Talk, IEICE Technical Committee on Internet Architecture (IA), 3 December 2026 |
| [Japanese municipal websites: hosting and RPKI](https://ba-cybersecurity.com/research/jp-municipal-hosting-rpki/) | Dataset, Zenodo, doi:10.5281/zenodo.23692415 |

#### Radars and writing

| | |
|---|---|
| [Cyber Defense Observatory](https://ba-cybersecurity.com/) | Daily radars built from public sources: breaches disclosed in Japan and the US, ransomware, WAF rule updates, PHP2Shell, web infrastructure. Data archive: [ba-radar-data](https://github.com/otoinobuo/ba-radar-data) (CC BY 4.0) |
| [What an AWS WAF log can and cannot tell you](https://ba-cybersecurity.com/writing/aws-waf-logs) | Article |
| [Exposed endpoint? Assess it. Don't scope it out.](https://ba-cybersecurity.com/writing/assess-dont-scope-out) | Article |
| [PHP's two critical RCEs (CVE-2026-109618, CVE-2026-109619)](https://ba-cybersecurity.com/writing/php-rce-cve-2026-109618) | What a WAF can and cannot do |

#### Links

[Research](https://ba-cybersecurity.com/research/) · [ORCID 0009-0001-1445-3612](https://orcid.org/0009-0001-1445-3612) · [Google Scholar](https://scholar.google.com/citations?user=VAyhjUUAAAAJ) · [SSRN](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=13422298) 

<sub>Nobuo Otoi (乙井信男) as ba-cybersecurity.com</sub>
