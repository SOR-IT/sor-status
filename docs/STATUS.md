# SOR Program Status

<!-- Public status feed — updated on each handoff save.
     Contains no implementation detail, architecture, or process IP.
     Read by: https://sor-it.github.io/sor-status/ -->

## NETWORK_STATUS
| status | APPROVED |
| detail | OPNsense · Technitium DNS · Samba AD · Kanidm SSO · Caddy. Hardware on order. Prerequisite for AI pipeline production deployment. |

## NETWORK_MILESTONES
| approval | DONE | Program approved & funded | Budget approved. Hardware procurement authorized. |
| hardware | ACTIVE | Hardware procurement | Firewall · switches · server — on order |
| opnsense | WAIT | OPNsense firewall + VLAN segmentation | Foundation network layer |
| dns | WAIT | Technitium DNS + internal zones | Split-horizon DNS for AI pipeline endpoints |
| samba | WAIT | Samba AD domain | User accounts · group policy · file shares |
| kanidm | WAIT | Kanidm SSO | Single sign-on for all internal services |
| caddy | WAIT | Caddy reverse proxy | HTTPS termination · ai.sortrock.local |
| voip | WAIT | VoIP cutover | Phone system migration |
| phase2vlans | WAIT | Phase 2 VLANs | Pre-press · production floor · IoT · cameras |
| complete | WAIT | Network modernization complete | Quarterly maintenance cadence begins |

## AI_STATUS
| status | PENDING |
| detail | Phase 0 complete. GitHub repo live — 36 files, CI 16/16 green. Dev environment on MacBook Pro configured and verified. Hardware on order. |

## HARDWARE
| Server 1 | WARN | ⚠ Backorder 6–8 wk | Primary inference · text models · Open WebUI |
| Server 2 | OK | ✓ On order | Visual extraction · image models · 128 GB |
| Dev Workstation | READY | ✓ Configured | Development environment · Phase 1A |

## AI_MILESTONES
| planning | DONE | Planning & architecture complete | Executive summary · project plan · combined timeline |
| repo | DONE | GitHub repository live | 36 files · CI 16/16 green · main + staging branches |
| devenv | DONE | Dev environment configured | MacBook Pro · Python 3.12 · Ollama + Qwen3 8B · FastAPI verified |
| phase1a | ACTIVE | Phase 1A — Simple lane + Website RFQ | Waiting on: Excel rate tables · Azure AD app registration |
| phase1b | WAIT | Phase 1B — Recipe library seeding | Historical job extraction · VLM extraction · ChromaDB ingestion |
| phase2 | WAIT | Phase 2 — Full fabrication pipeline | Requires Mac Studio + Strix Halo hardware arrival |
| phase3 | WAIT | Phase 3 — Calibration & accuracy tuning | Monthly estimate vs actual · recipe library to 100+ entries |

## NEXT_ACTION
Owner provides Excel rate table files (SOR_Rate_Table.xlsx, SOR_Recipe_Costs.xlsx, SOR_Markup_Schedule.xlsx) to begin Phase 1A. Build import_rates.py, stages/simple_lane.py, exception logic, and FastAPI routes. Azure AD app registration for Office 365 Graph API runs in parallel (docs/azure_ad_setup.md in private repo).
