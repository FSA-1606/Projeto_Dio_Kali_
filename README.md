# 🛡️ Relatório de Pentest – 192.168.56.101

Sobre o Projeto
Este repositório contém o relatório completo do teste de penetração realizado no alvo **192.168.56.101**. O documento detalha a enumeração de serviços, ataques de força bruta, exploração de vulnerabilidades e recomendações de mitigação.  

O relatório completo está disponível em PDF: [Relatório de Pentest](Relatorio Final Kali_Dio)

Análise de Vulnerabilidades
Durante o teste, foram identificadas as seguintes vulnerabilidades:

- **FTP:** Credenciais fracas detectadas (usuário: `msfadmin`, senha: `msfadmin`)  
- **Formulário Web (DVWA):** Login vulnerável a força bruta (usuário: `admin`, senha: `password`)  
- **SMB:** Acesso permitido com credenciais fracas (usuário: `msfadmin`, senha: `msfadmin`)  
- **Serviços abertos:** Portas críticas expostas (21, 22, 80, 139, 445)  

Essas vulnerabilidades permitem acesso não autorizado e exfiltração de dados.



Ferramentas Utilizadas
- **Nmap** – Varredura e enumeração de portas e serviços  
- **Medusa** – Ataques de força bruta em FTP e formulários web  
- **Hydra** – Ataques de força bruta em formulários web  
- **Enum4linux** – Enumeração SMB  
- **smbclient** – Acesso a compartilhamentos SMB  

Passos de Mitigação
Para reduzir riscos e corrigir vulnerabilidades detectadas:

1. **Alterar senhas fracas** em todos os serviços identificados.  
2. **Restringir acesso** apenas a IPs confiáveis ou redes internas.  
3. **Habilitar logs detalhados** para monitoramento de tentativas de login.  
4. **Implementar políticas de senha forte** e autenticação multifator (MFA) quando possível.  
5. **Fechar portas desnecessárias** e restringir exposição de serviços críticos à internet.  
6. **Monitoramento contínuo** de acessos e auditorias regulares de segurança.


Elaborado por: Fernando Andrade
Desafio DIO Cyber Security Santander
