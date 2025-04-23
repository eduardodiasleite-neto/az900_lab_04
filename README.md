# az900_lab_04
Construindo Arquiteturas no Azure.

Princípios para Construção de Arquiteturas no Azure <br>
1. Escalabilidade<br>
Azure oferece recursos como Auto-scaling (escalabilidade automática) para ajustar a infraestrutura conforme a demanda do aplicativo. Isso pode ser feito em níveis de máquinas virtuais, web apps e bancos de dados.<br>
Escalabilidade Horizontal: Adicionar mais instâncias para lidar com mais tráfego (exemplo: múltiplas VMs, containers ou instâncias de banco de dados).<br>
Escalabilidade Vertical: Aumentar os recursos de uma instância existente (exemplo: aumentar memória ou CPU de uma VM).<br>

2. Alta Disponibilidade e Resiliência<br>
Zona de Disponibilidade e Regiões Azure: Garantem que seus recursos sejam distribuídos geograficamente para evitar interrupções de serviço.<br>
Failover e Redundância: Usar recursos como Geo-redundant Storage (GRS) e Load Balancers para garantir a continuidade em caso de falha.<br>
Backup: Serviços como Azure Backup e Site Recovery para garantir recuperação em caso de falhas críticas.<br>

3. Segurança e Governança<br>
Identity Management: O Azure Active Directory permite controlar o acesso aos recursos e proteger suas identidades.<br>
Network Security: Utilização de Network Security Groups (NSGs), firewalls, Azure DDoS Protection e Web Application Firewall (WAF) para proteger a rede e dados.<br>
Políticas e Conformidade: O Azure Policy permite definir e aplicar políticas para conformidade e governança, garantindo que as melhores práticas de segurança sejam seguidas.<br>

4. Custo e Otimização<br>
Monitoramento de Custos: Ferramentas como Azure Cost Management e Azure Pricing Calculator ajudam a monitorar, estimar e otimizar os custos dos serviços no Azure.<br>
Uso de Preços Reservados e Escalabilidade Sob Demanda: Ajuste de recursos conforme o uso para equilibrar desempenho e custos.<br>

Exemplo de Arquitetura no Azure<br>
Arquitetura de Alta Disponibilidade para uma Aplicação Web<br>
Frontend: Uma aplicação web hospedada no Azure App Service com Azure CDN para entrega global.<br>
Backend: Azure SQL Database para dados relacionais, com Geo-Replication para alta disponibilidade.<br>
Escalabilidade: A VMs estão configuradas com escalabilidade automática através do Azure Load Balancer.<br>
Segurança: O acesso é controlado por Azure Active Directory e a comunicação entre os recursos usa VNet e NSGs.<br>
Monitoramento: Azure Monitor e Application Insights são usados para rastrear a performance da aplicação e identificar problemas.<br>
