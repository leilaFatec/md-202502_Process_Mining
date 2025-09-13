# Repositório da Disciplina – Entregas por Pull Request

Este repositório centraliza as **entregas dos grupos** da disciplina. **Ninguém faz push na `main`**: toda entrega deve ser feita via **Pull Request (PR)** a partir de um **fork**.

## 📦 Fluxo de Entrega (obrigatório)

1. Faça um **fork** deste repositório para a sua conta no GitHub.
2. Crie uma **branch** no seu fork usando o padrão:
   ```
   grupo-x/entrega-01
   ```
3. Adicione os arquivos **apenas** dentro do diretório do seu grupo e entrega, por exemplo:
   ```
   grupos/grupo-x/entrega-01/
   ```
4. Faça `commit` e `push` no **seu fork**.
5. Abra um **Pull Request** do seu fork para este repositório (base: `main`).
6. Preencha o **template de PR** (obrigatório) e aguarde a revisão do professor.
7. Se for solicitado ajuste, faça novos commits na **mesma branch** do seu fork.
8. Após **Approve**, o professor fará o merge.

> Dica: use nomes de arquivo autoexplicativos e inclua um `README.md` dentro da pasta da entrega explicando como executar/testar.

## 🗂️ Estrutura de Pastas (exemplo)
```
/
├─ grupos/
│  ├─ grupo-1/
│  │  ├─ entrega-01/
│  │  │  ├─ README.md        # instruções da entrega
│  │  │  └─ artefatos...     # código/diagramas/dados
│  │  └─ README.md           # info fixa do grupo (integrantes, papéis etc.)
│  ├─ grupo-2/
│  └─ ...
├─ .github/
│  ├─ CODEOWNERS
│  └─ pull_request_template.md
└─ README.md (este arquivo)
```

### Convenções
- **Branch**: `grupo-x/entrega-YY` (ex.: `grupo-3/entrega-02`)
- **Diretório da entrega**: `grupos/grupo-x/entrega-YY/`
- **Arquivos grandes**: evite subir binários pesados. Se necessário, use links para releases/drive.

## ✅ Regras de PR
- PRs **devem** alterar apenas diretórios do próprio grupo.
- Preencher o template é **obrigatório**.
- Discussões no PR devem ser **resolvidas** antes do merge.
- A `main` é **protegida**: só o professor pode aprovar e mergear.

## 🔒 Proteções (admin)
No repositório, ative em **Settings → Branches** (branch `main`):
- Require pull request before merging (1 approval)
- Require review from Code Owners
- Require conversation resolution before merging
- Block force pushes e deletions
- Restrict who can push (deixe sem colaboradores)

Crie/edite `.github/CODEOWNERS` para o @ do professor.

---

**Bom trabalho!**
