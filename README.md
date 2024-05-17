| Szenario / Kriterium             | Flux v2                                                 | ArgoCD                                                        |
|----------------------------------|---------------------------------------------------------|---------------------------------------------------------------|
| **Installation**                 | ✅ Klarer Einstieg, Verweise nach der Installation       | ⚠️ mangelnde Unterstützung nach der Installation              |
| **Bootstrapping**                | ✅ standardmäßig über Flux CLI                           | ✅ argocd-autopilot                                            |
| **CRD / Pruning**                | ✅ unterstützt                                           | ✅ unterstützt                                                 |
| **GUI / CLI**                    | ⚠️ Weniger Funktionalitäten                              | ✅ Viele Funktionalitäten                                      |
| **Zugriff auf Ressourcen via UI**| ⛔ nicht unterstützt, nur über CLI                       | ✅ unterstützt                                                 |
| **Self Healing**                 | ⚠️ Voll (aber Helm manuelle Änderungen nötig). Standardmäßig nicht vorhanden | ✅ Volle Unterstützung (standardmäßig deaktiviert)            |
| **Ignore Rules / Diffs**         | ⚠️ nur für Helm Releases                                 | ✅ Auf System- und Application Ebene                           |
| **Berechtigungen**               | ⚠️ kein eigenes Management System (Kubernetes nativ über Kubeconfig), SSO für UI | ✅ eigenes System (RBAC), SSO für UI und CLI                  |
| **Observability**                | ⚠️ Monitoring, Alerting, Notification Controller (27 Provider), kein SMTP (nur über Workarounds) | ⚠️ Monitoring, Alerting, Notification Controller (19 Provider), SMTP, keine git commit Status updates |
| **CMT**                          | ✅ Helm (über CLI erreichbar), Kustomize                  | ⚠️ Helm (über Helm CLI nicht erreichbar), Kustomize           |
| **OCI-Artifacts**                | ✅ unterstützt                                           | ⛔ nicht unterstützt                                           |
| **Patterns & Best Practices**    | ⚠️ Multi-cluster support, Repo Support, Keine Dokumentation oder Hinweise zu “Instance per namespace” | ✅ Multi-cluster support, Repo Support, Instance per Namespace |

