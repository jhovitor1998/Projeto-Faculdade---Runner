# Plano Revisado #2

## Premissas

- CLIs serão desenvolvidos em **Go** (1.25), por nativamente lidar com cross-compiling e as funcionalidades exigidas serem bem suportadas pela biblioteca padrão.
- O **assinador.jar** será desenvolvido em **Java 21**, por restrição de projeto.
- Estratégia **iterativa e incremental**, organizada em **4 sprints de 1 semana**.
- Cada sprint entrega valor ao usuário ou remove riscos técnicos relevantes.
- As histórias abaixo são subdivisões dos épicos US-01 a US-05 da [especificação](../especificacao.md), nomeadas como `US-XX.Y` indicando a história de origem.

## Rastreabilidade Épicos → Histórias

| Épico | Descrição | Histórias derivadas |
|-------|-----------|---------------------|
| US-01 | Invocar assinador.jar via CLI | US-01.1, US-01.2, US-01.3, US-01.4, US-01.5, US-01.6, US-01.7, US-01.8, US-01.9 |
| US-02 | Simular assinatura digital com validação | US-02.1, US-02.2, US-02.3, US-02.4, US-02.5 |
| US-03 | Gerenciar Ciclo de Vida do Simulador | US-03.1, US-03.2, US-03.3, US-03.4 |
| US-04 | Provisionar JDK Automaticamente | US-04.1 |
| US-05 | Disponibilizar binários multiplataforma | US-05.1, US-05.2, US-05.3 |

---

## Sprint 1 — Fundação e Entrega Contínua

**Objetivo:** Estabelecer a infraestrutura de desenvolvimento e entrega contínua.

### US-01.1 — Estrutura base do CLI em Go

**Critérios de aceitação:**
- [ ] Projeto Go inicializado com `go mod init github.com/kyriosdata/assinatura`
- [ ] Instalar ferramenta CLI em Go `go install github.com/spf13/cobra-cli@latest`
- [ ] Implementar comando `version`
- [ ] Estrutura de pacotes definida e documentada
- [ ] Aplicação compila nas três plataformas
- [ ] Comando `assinatura version` funcionando

### US-05.1 — Pipeline CI/CD multiplataforma

**Critérios de aceitação:**
- [ ] GitHub Actions configurado
- [ ] Cross-compilation para Windows, Linux e macOS
- [ ] Build a cada push
- [ ] Artefatos disponíveis no workflow

### US-05.2 — Publicação de releases

**Critérios de aceitação:**
- [ ] Versionamento SemVer (`v0.1.0`)
- [ ] Workflow de release configurado
- [ ] Binários publicados automaticamente
- [ ] Nome padrão dos artefatos definido

### US-05.3 — Checksums e assinatura

**Critérios de aceitação:**
- [ ] Geração de SHA256
- [ ] Assinatura com Cosign
- [ ] Arquivos `.sig` e `.pem`
- [ ] Processo automatizado
- [ ] Documentação de verificação

---

## Sprint 2 — Assinatura Digital (modo local)

### US-02.1 — Simulação de assinatura

**Critérios de aceitação:**
- [ ] Projeto Java inicializado
- [ ] Interface `SignatureService`
- [ ] Implementação fake
- [ ] Resposta simulada
- [ ] Testes unitários

### US-02.2 — Validação de parâmetros

**Critérios de aceitação:**
- [ ] Validação completa de parâmetros
- [ ] Mensagens de erro claras
- [ ] Rejeição de inválidos
- [ ] Testes

### US-02.3 — Validação de assinatura

**Critérios de aceitação:**
- [ ] Validação de entrada
- [ ] Retorno válido/inválido
- [ ] Mensagens claras
- [ ] Testes

### US-01.2 — CLI comandos

**Critérios de aceitação:**
- [ ] Comando `sign`
- [ ] Comando `validate`
- [ ] `--help`
- [ ] Tratamento de erro
- [ ] Testes

### US-01.3 — Invocar jar

**Critérios de aceitação:**
- [ ] Executar `java -jar`
- [ ] Mapear parâmetros
- [ ] Capturar saída
- [ ] Tratar erros
- [ ] Testes

### US-01.4 — Exibição de resultados

**Critérios de aceitação:**
- [ ] Saída legível
- [ ] Indicação de válido/inválido
- [ ] Erros claros
- [ ] Uso fácil no terminal

### US-04.1 — Provisionar JDK

**Critérios de aceitação:**
- [ ] Detectar JDK
- [ ] Baixar se necessário
- [ ] Cache local
- [ ] Evitar download duplicado
- [ ] Testes

---

## Sprint 3 — Modo Servidor

(Tudo ainda pendente)

---

## Sprint 4 — Simulador

(Tudo ainda pendente)

---

## 📌 Status Geral

🚧 Projeto ainda **não iniciado**  
📅 Planejamento concluído, execução começará na Sprint 1
