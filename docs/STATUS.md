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
| detail | Phase 0 complete. Repo live — 36 files, CI 16/16 green. Dev environment verified. Pending funding approval and rate table files to begin Phase 1A. |

## AI_MILESTONES
| p0_planning | DONE | Phase 0 — Planning & architecture complete | Decisions locked · documents in repo · funding proposal submitted |
| p0_repo | DONE | Phase 0 — GitHub repository live | 36 files · CI 16/16 green · main + staging branches |
| p0_devenv | DONE | Phase 0 — Dev environment configured | MacBook Pro · Python 3.12 · Ollama + Qwen3 8B · FastAPI verified |
| p0_dashboard | DONE | Phase 0 — Status dashboard live | sor-it.github.io/sor-status · auto-updates on handoff save |
| p1a_rates | ACTIVE | Phase 1A — Rate tables (owner action) | Excel files required before pipeline pricing can be built or tested |
| p1a_azuread | ACTIVE | Phase 1A — Azure AD app registration (owner action) | Office 365 Graph API · quotes@ shared mailbox |
| p1a_simple | WAIT | Phase 1A — Simple lane CSR path | import_rates.py · simple_lane.py · exception_logic.py · FastAPI routes |
| p1a_rfq | WAIT | Phase 1A — Website RFQ auto-send | mail/parser.py tuned · auto-send + escalation tested end-to-end |
| p1a_live | WAIT | Phase 1A — Production deployment | 20+ real jobs · 5+ auto-sent quotes · promotion checklist executed |
| p1b_seed | WAIT | Phase 1B — Recipe library seeding | Historical DM jobs extracted · 10–15 entries · 3 design families |
| p1b_accuracy | WAIT | Phase 1B — Accuracy baseline | 3 historical jobs tested · estimate vs actual ±15% target |
| p2_hw | WAIT | Phase 2 — Hardware installation | Server 1 (Mac Studio) + Server 2 (Strix Halo) configured |
| p2_stages | WAIT | Phase 2 — Fabrication pipeline stages A–H | All 8 stages built · staged in CI · integration tested |
| p2_dashboard | WAIT | Phase 2 — Stage G review dashboard | api.sortrock.local/review/{job_id} · PM approval gate |
| p2b_pitstop | WAIT | Phase 2B — PitStop translation | Switch Script node → FastAPI → client email draft |
| p2_live | WAIT | Phase 2 — Production deployment | Internal beta complete · manual workflow retired for familiar families |
| p3_calibrate | WAIT | Phase 3 — Calibration & accuracy tuning | Monthly estimate vs actual · recipe library to 100+ entries |

## HARDWARE
| Server 1 | WARN | ⚠ Backorder 6–8 wk | Primary inference · text models · Open WebUI |
| Server 2 | OK | ✓ Arrived — pending setup | Visual extraction · image models · 128 GB |
| Dev Workstation | READY | ✓ Configured | Development environment · Phase 1A |

## NEXT_ACTION
Owner provides Excel rate table files (SOR_Rate_Table.xlsx, SOR_Recipe_Costs.xlsx, SOR_Markup_Schedule.xlsx) to begin Phase 1A. In parallel: Azure AD app registration for Office 365 Graph API — documented in project repo. Both are owner actions that unblock all Phase 1A code work.
