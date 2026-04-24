# Places - Sistema de Diretório de Negócios

![Laravel](https://img.shields.io/badge/Laravel-12.x-FF2D20?style=for-the-badge&logo=laravel)
![PHP](https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php)

O **Places** é uma aplicação web desenvolvida em Laravel para a gestão e listagem de negócios locais organizados por categorias.

## 🚀 Estado Atual do Projeto

O projeto encontra-se em fase inicial de desenvolvimento, com a estrutura base de dados e lógica de backend essencial já implementadas.

### Funcionalidades Implementadas:
- **Gestão de Categorias**: Sistema para organizar negócios (ex: Restaurantes, Oficinas, Lojas).
- **Base de Dados de Negócios**: Estrutura completa para armazenar:
  - Nome do negócio
  - Morada
  - NIF (VAT Number)
  - Contactos (Telefone e Email)
  - Estado (Ativo/Inativo)
  - Associação a uma categoria específica.
- **API/Controller**: `CategoryController` já configurado com métodos para listagem.

## 🛠️ Tech Stack

- **Framework:** Laravel 12
- **Linguagem:** PHP 8.2+
- **Frontend:** Blade Templates & Tailwind CSS (via Vite)
- **Base de Dados:** SQLite (padrão para desenvolvimento)

## 📦 Instalação e Configuração

Para configurar o projeto localmente, siga estes passos:

1. **Clonar o repositório:**
   ```bash
   git clone <url-do-repositorio>
   cd places
   ```

2. **Executar o script de configuração automática:**
   O projeto inclui um comando personalizado no `composer.json` que automatiza a instalação de dependências, criação do `.env`, geração da chave e migrações:
   ```bash
   composer run setup
   ```

3. **Iniciar o servidor de desenvolvimento:**
   O projeto utiliza o `concurrently` para correr o servidor Laravel e o Vite em simultâneo:
   ```bash
   composer run dev
   ```

## 📂 Estrutura de Rotas Principais

- `/` - Página de boas-vindas.
- `/categories` - Listagem e gestão de categorias.

## 📝 Notas de Desenvolvimento

- O projeto utiliza migrações modernas do Laravel 12.
- A base de dados SQLite é criada automaticamente durante o processo de `setup`.
- O sistema de autenticação base do Laravel está pronto a ser configurado/utilizado se necessário.

---
Desenvolvido por Diogo Pimenta.
