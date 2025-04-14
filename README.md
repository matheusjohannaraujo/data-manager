# DataManager

**DataManager** é uma biblioteca PHP desenvolvida para simplificar a manipulação de arquivos e diretórios, oferecendo uma interface intuitiva para operações comuns no sistema de arquivos.

## 📦 Instalação

Você pode instalar a biblioteca via Composer:

```bash
composer require mjohann/data-manager
```

## ⚙️ Requisitos

- PHP 7.0 ou superior

## 🚀 Funcionalidades

- Criação, leitura, atualização e exclusão de arquivos
- Criação e exclusão de diretórios
- Listagem de arquivos e diretórios
- Verificação de existência de arquivos ou diretórios
- Leitura e escrita de conteúdo em arquivos
- Renomear arquivos e diretórios
- Obtenção de informações detalhadas sobre arquivos

## 🧪 Exemplo de Uso

```php
use MJohann\Packlib\DataManager;

DataManager::folderCreate("my_dir");

DataManager::fileCreate("my_dir/file.txt", "Test DataManager");

echo DataManager::fileRead("my_dir/file.txt");

echo DataManager::size("my_dir/");

```

Para mais exemplos, consulte o arquivo [`example/script.php`](example/script.php) no repositório.

## 📁 Estrutura do Projeto

```
data-manager/
├── src/
│   └── DataManager.php
├── example/
│   └── script.php
├── LICENSE
└── README.md
```

## 📄 Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais informações.

## 👨‍💻 Autor

Desenvolvido por [Matheus Johann Araújo](https://github.com/matheusjohannaraujo) - Pernambuco, Brasil.