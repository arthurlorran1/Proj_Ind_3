# Resiliadata - 
Um oferecimento Arthur Lorran

### 1. Entidades Necessárias
- EmpresasParceiras
- Tecnologias
- TecnologiasEmpresas
- Colaboradores

### 2. Principais Campos e Tipos
**EmpresasParceiras:**
- `id_empresa` (INT)
- `nome_empresa` (VARCHAR)
- `endereco` (VARCHAR)
- `contato` (VARCHAR)

**Tecnologias:**
- `id_tecnologia` (INT)
- `nome_tecnologia` (VARCHAR)
- `area_tecnologia` (VARCHAR)

**TecnologiasEmpresas:**
- `id_relacao` (INT)
- `id_empresa` (INT)
- `id_tecnologia` (INT)

**Colaboradores:**
- `id_colaborador` (INT)
- `nome_colaborador` (VARCHAR)
- `cargo` (VARCHAR)
- `id_empresa` (INT)

### 3. Relacionamentos
- EmpresasParceiras possui relação com TecnologiasEmpresas através de `id_empresa`.
- Tecnologias possui relação com TecnologiasEmpresas através de `id_tecnologia`.
- Colaboradores possui relação com EmpresasParceiras através de `id_empresa`.
