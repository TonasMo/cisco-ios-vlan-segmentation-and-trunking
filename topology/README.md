Laboratório prático de configuração de **VLANs**, alteração de **VLAN Nativa** e estruturação de **Link Trunk** entre dois switches Cisco em ambiente de simulação.

## 📐 Especificações da Rede

### Tabela de VLANs
| VLAN ID | Nome da VLAN | Atribuição |
| :--- | :--- | :--- |
| **20** | HR | SW-1 |
| **40** | Admin | SW-1 e SW-2 |
| **50** | NativeVLAN | SW-1 e SW-2 (Nativa no Trunk) |
| **80** | IT | SW-2 |

---

## ⛓️ Configuração da Interconexão Trunk

- **Interface Utilizada:** `GigabitEthernet0/1` em ambos os switches
- **Modo:** Trunk (`dot1q`)
- **VLAN Nativa:** `VLAN 50`
- **VLANs Permitidas:** `20, 40, 50, 80`

## Validação

- show vlan brief
- show interfaces trunk