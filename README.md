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

### Configuração do Flutter SDK

O Flutter **não é mais utilizado como submódulo**. Para configurar o ambiente do frontend, siga os passos abaixo:

1. Baixe ou clone o SDK do Flutter na pasta `unigo-frontend/flutter`:
```bash
git clone https://github.com/flutter/flutter.git -b stable unigo-frontend/flutter
```

2. Adicione o Flutter ao seu PATH (recomendado):
   - No Windows, adicione `C:\Users\<seu-usuario>\Desktop\unigo-project\unigo-frontend\flutter\bin` ao PATH do sistema.
   - No Linux/Mac, adicione ao seu `.bashrc` ou `.zshrc`:
     ```bash
     export PATH="$(pwd)/unigo-frontend/flutter/bin:$PATH"
     ```

3. Verifique a instalação:
```bash
cd unigo-frontend
./flutter/bin/flutter doctor
```

4. Instale o Android Studio e configure o SDK do Android, se desejar desenvolver para Android.

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