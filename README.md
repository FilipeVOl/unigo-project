# Unigo Project

Este é o repositório principal do projeto Unigo, que contém tanto o backend quanto o frontend da aplicação.

## Estrutura do Projeto

O projeto está organizado em dois submódulos:

- `unigo-backend`: Backend da aplicação desenvolvido com Node.js, TypeScript e TypeORM
- `unigo-frontend`: Frontend da aplicação desenvolvido com Flutter

## Configuração do Ambiente

1. Clone o repositório com os submódulos:
```bash
git clone --recursive https://github.com/seu-usuario/unigo-project.git
cd unigo-project
```

2. Se você já clonou o repositório sem os submódulos, execute:
```bash
git submodule update --init --recursive
```

3. Configure as variáveis de ambiente:
   - Copie o arquivo `.env.example` para `.env` na raiz do projeto
   - Ajuste as variáveis conforme necessário

4. Inicie os serviços com Docker Compose:
```bash
docker-compose up -d
```

## Desenvolvimento

Para trabalhar com os submódulos:

1. Atualizar todos os submódulos:
```bash
git submodule update --remote
```

2. Trabalhar em um submódulo específico:
```bash
cd unigo-backend  # ou unigo-frontend
git checkout main
git pull origin main
```

## Contribuição

1. Faça suas alterações no submódulo apropriado
2. Commit e push das alterações no submódulo
3. Atualize a referência do submódulo no repositório principal
4. Commit e push das alterações no repositório principal

## Licença

Este projeto está sob a licença MIT. 